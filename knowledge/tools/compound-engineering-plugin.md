# Compound Engineering Plugin

**Repo:** EveryInc/compound-engineering-plugin
**Language:** Python
**Stars:** 5,296
**URL:** https://github.com/EveryInc/compound-engineering-plugin
**Creator:** Kieran Klaassen

Official Claude Code plugin that makes each unit of engineering work easier than the last.

## Installation

```bash
/plugin marketplace add https://github.com/EveryInc/compound-engineering-plugin
/plugin install compound-engineering
```

## Core Workflow

```
Plan → Work → Review → Compound → Repeat
```

## Commands

| Command | Purpose |
|---------|---------|
| `/workflows:plan` | Turn feature ideas into detailed implementation plans |
| `/workflows:work` | Execute plans with worktrees and task tracking |
| `/workflows:review` | Multi-agent code review before merging |
| `/workflows:compound` | Document learnings to make future work easier |

## Philosophy

Each unit of engineering work should make subsequent units easier—not harder.

Traditional development accumulates technical debt. The compound engineering approach inverts this:
- **80% planning and review, 20% execution**
- Plan thoroughly before writing code
- Review to catch issues and capture learnings
- Codify knowledge so it's reusable
- Keep quality high so future changes are easy

## Key Features

- **Agent-driven planning and review** - multiple agents analyze code and requirements
- **Worktree-based execution** - isolated branches for safe experimentation
- **Task tracking** - structured progress monitoring
- **Compound documentation** - learnings captured for future work

## Notable Integration

Kieran Klaassen replaced Playwright MCP with the agent-browser skill included in this plugin, eliminating 12k token overhead while improving browser automation capabilities.
