---
title: "banteg/agents - AI Agent Workflows"
type: tool
date_added: 2026-01-04
source: "https://github.com/banteg/agents"
author: "banteg"
tags: [ai-agents, claude-code, codex, devcontainer, git-worktrees, docker, workflow]
via: "Twitter bookmark from @banteg"
---

banteg/agents is a comprehensive collection of workflows and tools for running AI agents (Claude Code, Codex) safely and efficiently in isolated environments. It addresses the core challenge of agent development: isolation and controlled execution.

The repository provides opinionated tooling for the complete agent lifecycle: checking out work in isolated git worktrees, running agents unattended in devcontainers, and managing authentication across multiple repository contexts.

## Key Features

### Git Worktree Management
- **git-wt** - Simple wrapper for common git worktree operations
  - `git wt` - list all worktrees
  - `git wt feat/branch` - switch or create worktree
  - `git wt -d/-D` - soft/hard delete

- **worktrunk** - Full-featured worktree CLI with additional capabilities
  - Auto-running install scripts
  - Commit generation with llm CLI
  - PR workflow integration
  - Interactive worktree switching

- **Relative Worktree Paths** - Git 2.48+ support for relative paths (fixes devcontainer issues)

### Devcontainer Setup
- Official bunny devcontainer configuration
- Run Claude Code and Codex in "yolo mode" (unattended)
- Authentication persistence via shared Docker volumes
- Isolated execution environment
- Uses orbstack as recommended Docker replacement

### Code Review & Planning
- Git-based context delivery instead of repomix/code2prompt
- `git archive` for creating focused code zips
- `git bundle` support for commit history context
- Compatible with GPT Pro, Claude, and Gemini

### Notifications
- **takopi** integration - Telegram control of agents with progress streaming
- Resumable sessions (start on phone, continue in terminal)
- Install: `uv tool install takopi`

## Technical Details

- **Language:** Bash/Shell scripts
- **License:** MIT (inferred from GitHub)
- **Repository:** github.com/banteg/agents
- **Status:** Active development, production-ready
- **Key Dependency:** Docker (orbstack recommended)

## Installation

### Set up git worktrees
```bash
git config wt.basedir .worktrees
brew install k1LoW/tap/git-wt
```

### Enable relative worktree paths
```bash
git config --global worktree.useRelativePaths true
```

### Use devcontainer
```bash
./devcontainer/install.sh self-install
devc /path/to/repo
```

## Use Cases

- Running agents unattended on background tasks
- Isolating multiple agent branches to prevent interference
- Managing authentication across multiple repositories
- Integrating agent output with PR/review workflows
- Streaming agent progress via Telegram notifications

## Philosophy

The repository emphasizes "less is more" - simpler agent configurations lead to faster execution. Over-engineered agent files and skill directories actually hurt speed. The focus is on isolation (prevents agents from interfering with each other) and clean workflows.

## Links

- [GitHub Repository](https://github.com/banteg/agents)
- [Original Tweet](https://x.com/banteg/status/2007748646230733139)
- [git-wt](https://github.com/k1LoW/git-wt)
- [worktrunk](https://worktrunk.dev/)
- [takopi](https://github.com/banteg/takopi)
- [orbstack](https://orbstack.dev/)
