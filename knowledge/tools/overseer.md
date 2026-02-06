# Overseer

**GitHub:** https://github.com/dmmulroy/overseer | **Author:** Dillon Mulroy

Task orchestration system for AI agents via MCP. Built with Rust CLI + Node.js MCP server.

## Status
Early-stage but functional (as of Jan 2026). Not yet ready for public use.

## Core Architecture
- **CLI (Rust):** SQLite storage, task management, VCS integration
- **MCP Server (Node.js):** Single "execute" tool using codemode pattern where agents write JavaScript that runs in a sandbox
- **VCS:** Native support for jj-lib (primary) and git fallback

## Key Features

### Task Management
- Hierarchical tasks: Milestones (depth 0) → Tasks (depth 1) → Subtasks (depth 2)
- Task states: pending, ready, completed, blocked
- Priority, context, and blocking relationships
- Learning bubble-up (child learnings aggregate to parent on completion)

### Codemode Pattern
Agents interact via a single `execute` tool - they write JavaScript that the server executes:
```javascript
const milestone = await tasks.create({
  description: "User auth system",
  context: "JWT + refresh tokens"
});

const login = await tasks.create({
  description: "Login endpoint",
  parentId: milestone.id
});

await tasks.start(login.id);  // Creates VCS bookmark, records start commit
// ... work happens ...
await tasks.complete(login.id, {
  result: "Implemented with bcrypt",
  learnings: ["bcrypt rounds should be 12+ for production"]
});
```

### VCS Integration
- `tasks.start()` creates bookmark, records start commit (VCS required)
- `tasks.complete()` commits changes, deletes bookmark, bubbles learnings
- Best-effort cleanup on task deletion

### Progressive Context
Tasks inherit context from ancestors. Three context levels:
- `context.own` - This task's context
- `context.parent` - Parent task context
- `context.milestone` - Root milestone context

### CLI Tools
- Task CRUD: create, get, list, update, delete, reopen
- Workflow: start, complete, block/unblock
- Queries: next-ready, tree, search, progress
- VCS: detect, status, log, commit, cleanup
- Data export to JSON
- Web UI viewer (React/SvelteKit)

## Installation
```bash
npm install -g @dmmulroy/overseer
# or via skills.sh for agents:
npx skills add dmmulroy/overseer
```

## MCP Configuration
```json
{
  "mcpServers": {
    "overseer": {
      "command": "npx",
      "args": ["@dmmulroy/overseer", "mcp"]
    }
  }
}
```

## Notes
- SQLite backend provides persistent task state
- VM sandbox provides isolation for agent-written JavaScript
- Task learning system prevents "sandcastling" (decisions being forgotten/undone)
- VCS bookmarks track which tasks are currently being worked on
