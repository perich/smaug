# Ledger - Visual Git Worktree Manager

**Repository:** https://github.com/peterjthomson/ledger

A modernised git interface for macOS designed to improve agent and human collaboration, with special support for managing multiple AI coding agent workspaces (Cursor, Claude, Conductor).

## Key Features

- **Pull Request Integration** - View open PRs from GitHub, filter by status, see reviews and inline diffs
- **Worktree Support** - View and navigate git worktrees with detection for AI agent workspaces and change stats
- **Branch Management** - View local/remote branches with metadata, filter and sort capabilities
- **Commit & Staging** - View commit history with graph visualization, stage/unstage files with diffs
- **Stash Management** - View, apply, and pop stashes with preview
- **Opinionated Git** - Auto-stash for safe operations, PR preview for "virtual merge", leapfrog-style flows

## Tech Stack

- Electron (cross-platform desktop framework)
- React 19 (UI library)
- TypeScript (type-safe JavaScript)

## Platform Support

- macOS (Apple Silicon)
- Linux (Ubuntu/Debian x64, AppImage)
- Windows (NSIS installer)

## Requirements

- `git` available on PATH
- GitHub CLI (`gh`) - optional, for PR integration

## Use Case

Ideal for managing multiple concurrent coding sessions with AI agents, visualizing complex branch structures, and maintaining control over automated code changes.
