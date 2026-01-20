# Agent Scripts

Shared guardrail helpers and workflow scripts for AI agents across repositories.

**Repository:** [steipete/agent-scripts](https://github.com/steipete/agent-scripts)
**Stars:** 1243
**Language:** TypeScript

## What it is

Collection of reusable scripts and guardrails for managing agent workflows. Designed for multi-repo AI agent coordination with consistent patterns across projects.

## Core components

### Committer Helper (`scripts/committer`)
- Bash script that stages exactly the files you list
- Enforces non-empty commit messages
- Creates atomic commits with proper formatting

### Docs Lister (`scripts/docs-list.ts`)
- TypeScript script that walks `docs/` directory
- Enforces front-matter requirements (`summary`, `read_when`)
- Prints summaries for agent onboarding flows
- Compiled binary available in `bin/docs-list`

### Browser Tools (`bin/browser-tools`)
- Standalone Chrome/Chromium automation helper
- Launches/inspects DevTools-enabled Chrome profiles
- Pastes prompts, captures screenshots, manages stray processes
- No MCP required; zero repo-specific imports

### Skills

- `swift-concurrency-expert`
- `swiftui-liquid-glass`
- `swiftui-performance-audit`
- `swiftui-view-refactor`
- Additional custom skills as needed

## Pointer-style workflow

- Shared guardrail text lives in this repo: `AGENTS.MD`
- Downstream repos reference via pointer: `READ ~/Projects/agent-scripts/AGENTS.MD BEFORE ANYTHING`
- Repo-specific rules go after the pointer
- Keeps instructions DRY across multiple projects

## Sync expectations

This is the canonical mirror for guardrail helpers. When editing:
1. Update `scripts/committer`, `scripts/docs-list.ts`, or other helpers
2. Copy changes back to this repo immediately
3. Mirror changes to all downstream repos
4. Keep code byte-identical across mirrors
5. Submodules get their own pointer check

## Setup

```bash
# Clone the repo
git clone https://github.com/steipete/agent-scripts.git ~/Projects/agent-scripts

# Browser tools (if using)
bun build scripts/browser-tools.ts --compile --target bun --outfile bin/browser-tools

# In downstream repos, add to AGENTS.MD:
# READ ~/Projects/agent-scripts/AGENTS.MD BEFORE ANYTHING
```

## Use case

Streamline multi-repo AI agent workflows with consistent tooling, shared documentation patterns, and coordinated guardrails.
