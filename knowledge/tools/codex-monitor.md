# Codex Monitor

MacOS command center for orchestrating Codex agents across workspaces.

**Website:** https://www.codexmonitor.app/
**Repository:** [Dimillian/CodexMonitor](https://github.com/Dimillian/CodexMonitor)
**Built with:** Tauri + React
**Platform:** macOS + Linux

## What it is

A beautifully crafted macOS/Linux application that orchestrates multiple Codex agents across local workspaces. Keeps entire AI agent workflows in one surface with threads, reviews, diffs, and git integration.

## Core features

### Workspace Orchestration
- Add, persist, and reconnect workspaces
- Live dashboard of recent activity
- Multiple agents in one view

### Thread Control
- Start threads and resume history
- Handle approvals without context switching
- Chat interface with integrated context

### Worktree Agents
- Spin up per-branch worktrees for isolated changes
- Clean review workflows
- Automatic branch management

### Git + GitHub Integration
- Diffs, logs, branch controls
- Issues via `gh` CLI built-in
- Commit history and review tools

### Model + Access Controls
- Pick models per run
- Tune reasoning effort (high/xhigh)
- Lock in access modes

### Plans and Reviews
- Track per-turn plans
- Run reviews directly in app
- Export debug logs on demand

### Skills + Prompts
- Autocomplete for skills
- Prompt templates
- File token management

### Polish + Updates
- Toast-driven updates
- Resizable panels
- macOS overlay title bar
- Beautiful glass morphism design

## Architecture

- **Frontend:** React
- **Backend:** Tauri (native desktop framework)
- **Language:** TypeScript/Rust

## Workflow

1. **Connect workspaces** - Launch Codex app-server per repo, restore threads
2. **Run agent** - Pick models, access mode, and skills; chat in one view
3. **Review + ship** - Open diffs, logs, and reviews alongside threads

## Use case

For teams and individuals shipping code with AI agents. Codex Monitor replaces scattered CLI sessions and terminal contexts with a unified orchestration center designed for fast, visible, and organized AI-powered development workflows.

## Getting started

- Download from [GitHub Releases](https://github.com/Dimillian/CodexMonitor/releases)
- View source on [GitHub](https://github.com/Dimillian/CodexMonitor)
- Read [changelog](https://www.codexmonitor.app/changelog.html)

## Key differentiator

This is not an IDE. Codex Monitor intentionally excludes a built-in text editor because developers already have good editors. Instead, it focuses on what it does best: orchestrating, monitoring, and coordinating AI agent runs across your actual projects.
