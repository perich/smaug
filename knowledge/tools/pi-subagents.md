# pi-subagents

**URL:** https://github.com/nicobailon/pi-subagents

**Author:** nicobailon

**Stars:** 88

**Language:** TypeScript

## Summary

Pi extension for delegating tasks to subagents with chains, parallel execution, TUI clarification, and async support. Enables building complex agent systems with specialized subagents that can be orchestrated synchronously or asynchronously.

## Key Features

- **Agent definitions** — Markdown files with YAML frontmatter declaring specialized configurations
- **MCP tool integration** — Agents can use MCP server tools directly (requires pi-mcp-adapter)
- **Skill injection** — Agents declare skills in frontmatter; skills get injected into system prompts
- **Chain orchestration** — Sequential task chains with variable interpolation ({task}, {previous}, {chain_dir})
- **Parallel execution** — Fan-out/fan-in patterns with parallel steps within chains
- **TUI clarification** — Interactive preview/edit of chain templates before execution
- **Async support** — Background execution with durable status tracking and async widgets
- **Session sharing** — Inter-step file sharing via chain artifacts directory
- **Progress tracking** — Real-time visibility during execution with token counting and duration tracking
- **Output management** — Configurable byte/line limits and debug artifact generation

## Agent File Structure

Agents are markdown files with YAML frontmatter:

```yaml
---
name: scout
description: Fast codebase recon
tools: read, grep, find, ls, bash, mcp:chrome-devtools
model: claude-haiku-4-5
skill: safe-bash, chrome-devtools
output: context.md
defaultReads: context.md
defaultProgress: true
---

Your system prompt goes here.
```

## MCP Tool Configuration

Agents can reference MCP tools with `mcp:` prefix:
- `mcp:server-name` — All tools from a server
- `mcp:server-name/tool_name` — Specific tool

## Modes

| Mode | Async | Description |
|------|-------|-------------|
| Single | Yes | Execute one agent ({agent, task}) |
| Chain | Yes* | Sequential task execution with variable passing |
| Parallel | Sync only | Multiple tasks in parallel (auto-downgrades if async requested) |

## Installation

```bash
pi install npm:pi-subagents
```

## Use Cases

- Building specialized agent teams for different tasks
- Orchestrating complex workflows with agent chains
- Delegating work to background agents with async execution
- Integrating MCP tools with subagent-specific configurations
- Interactive chain composition and clarification before execution

## Related

- **pi-mcp-adapter** — Provides efficient MCP tool loading for subagents
