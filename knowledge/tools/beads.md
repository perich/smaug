---
title: "Beads"
type: tool
date_added: 2026-01-05
source: "https://github.com/steveyegge/beads"
tags: [agents, claude-code, coding, task-management, git-backed, issue-tracking]
via: "Twitter bookmark from @0xfdf"
---

Beads (bd) is a distributed, git-backed graph issue tracker specifically designed for AI agents. It provides persistent memory and structured task management for coding agents, solving the challenge of maintaining context and dependencies across multi-session workflows.

## Key Features

- **Git as Database** - Issues stored as JSONL in `.beads/`. Versioned, branched, and merged like code.
- **Agent-Optimized** - JSON output, dependency tracking, and auto-ready task detection
- **Zero Conflict** - Hash-based IDs prevent merge collisions in multi-agent/multi-branch workflows
- **Invisible Infrastructure** - SQLite local cache for speed; background daemon for auto-sync
- **Compaction** - Semantic "memory decay" summarizes old closed tasks to save context window
- **GitHub Integration** - Sync issues to GitHub with preserved hierarchy using `gh` tool
- **Hierarchical Structure** - Support for epics and nested tasks (bd-a3f8, bd-a3f8.1, etc.)
- **Dependency Awareness** - Track blockers, related tasks, and parent-child relationships

## Essential Commands

| Command | Action |
| --- | --- |
| `bd ready` | List tasks with no open blockers |
| `bd create "Title" -p 0` | Create a P0 task |
| `bd dep add <child> <parent>` | Link tasks |
| `bd show <id>` | View task details and audit trail |

## Installation

- **npm:** `npm install -g @beads/bd`
- **Homebrew:** `brew install steveyegge/beads/bd`
- **Go:** `go install github.com/steveyegge/beads/cmd/bd@latest`

## Use Cases

- Multi-session development with state carryover
- Coordinating multiple AI agents for complex tasks
- Research and experimentation workflows
- Token-efficient long-running agent systems
- Tracking work across feature branches and distributed teams

## Technical Details

- **Language:** Go (with npm and Homebrew packages available)
- **Repository:** github.com/steveyegge/beads
- **Stars:** 8,287+
- **Requirements:** Linux (glibc 2.32+), macOS, or Windows

## Community Tools

See the repository for curated list of community-built UIs, extensions, and integrations including terminal interfaces, web UIs, editor extensions, and native apps.

## Links

- [GitHub](https://github.com/steveyegge/beads)
- [Documentation](https://github.com/steveyegge/beads)
- [Original Tweet](https://x.com/0xfdf/status/2006807995884175661)
