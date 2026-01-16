# claude-code-config

**Author:** jarrodwatts
**GitHub:** https://github.com/jarrodwatts/claude-code-config
**Stars:** 812
**Language:** JavaScript

A comprehensive personal Claude Code configuration repository that includes agents, commands, hooks, rules, skills, and plugins for enhanced development workflow.

## Overview

This repository contains curated Claude Code configurations sourced from the community, providing ready-to-use enhancements for development work.

## Installation Options

1. **Copy-Paste into Claude Code** - Copy the prompt from INSTALL.md and Claude will fetch all config files automatically
2. **Git Clone** - `git clone https://github.com/jarrodwatts/claude-code-config.git ~/.claude`
3. **Selective Install** - Clone and selectively copy specific rules, skills, or agents

## Components

### Rules (.claude/rules/)
Path-scoped instructions loaded automatically for matching files:
- TypeScript conventions
- Testing patterns
- Comment policy
- Foundry/ZKsync rules

### Skills (.claude/skills/)
- `planning-with-files` - Manus-style persistent markdown planning

### Agents (.claude/agents/)
- `codebase-search` - Find files and implementations
- `media-interpreter` - Extract info from PDFs/images
- `open-source-librarian` - Research OSS with citations
- `tech-docs-writer` - Create technical documentation

### Commands (.claude/commands/)
- `interview` - Interactive planning/spec fleshing

### Hooks (.claude/hooks/)
- `keyword-detector.py` - Detects keywords in prompts
- `check-comments.py` - Validates comment policy
- `todo-enforcer.sh` - Ensures todos are tracked

## Recommended Plugins

Official plugins:
- frontend-design
- code-review
- typescript-lsp
- plugin-dev
- ralph-loop
- claude-hud (status line)

## Tags
[[claude-code]] [[developer-tools]] [[configuration]] [[dotfiles]] [[ai]]
