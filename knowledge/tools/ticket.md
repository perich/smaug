# Ticket - Git-Native Issue Tracker

**Repository:** https://github.com/wedow/ticket

A minimal, git-backed issue tracking system designed specifically for AI agents, written as a bash script in under 1500 lines. Inspired by Unix Philosophy and Joe Armstrong's Minimal Viable Program concept.

## Key Features

- **Markdown + YAML Frontmatter** - Tickets stored as `.tickets/*.md` files with YAML metadata for easy AI search and IDE navigation
- **Dependency Tracking** - Complex issue dependency graphs with cycle detection
- **Priority Levels** - 5-level priority system (0-4, with 0 being highest)
- **Ticket Types** - Supports bug, feature, task, epic, chore
- **Status Management** - open, in_progress, closed states
- **Tagging System** - Organize tickets with tags
- **CLI Commands** - Full command-line interface with bash completion

## Common Commands

```bash
tk create "Title" -d "Description" -t feature -p 2
tk start <id>
tk close <id>
tk dep <id> <dep-id>  # Add dependency
tk dep tree <id>      # Show dependency tree
tk ready              # List tickets with resolved deps
tk blocked            # List tickets with unblocked deps
```

## Installation

**Homebrew:**
```bash
brew tap wedow/tools
brew install ticket
```

**From source:**
```bash
git clone https://github.com/wedow/ticket.git
cd ticket && ln -s "$PWD/ticket" ~/.local/bin/tk
```

## Requirements

- POSIX-compliant bash (portable across macOS, Linux, Windows with WSL)
- `jq` for query command
- `rg` (ripgrep) preferred, falls back to `grep`

## Use Case

Perfect for AI agents managing their own task workflows, with dependency tracking designed to prevent agents from working on blocked tasks. The markdown format allows AI to read/understand tickets without context window bloat.

## Agent Integration

Add to project documentation:
```
This project uses a CLI ticket system for task management. Run `tk help` when you need to use it.
```

Claude Opus naturally picks up this pattern from documentation.
