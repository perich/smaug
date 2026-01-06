---
title: "Flow Plugin"
type: tool
date_added: 2026-01-05
source: "https://github.com/gmickel/gmickel-claude-marketplace"
tags: [claude-code, workflow, planning, code-review, execution, marketplace]
via: "Twitter bookmark from @gmickel"
---

Flow is a Claude Code plugin from Gordon Mickel that implements a disciplined plan-first workflow for AI-driven development. It addresses common AI agent failure modes through structured planning, parallel research, pattern reuse, and cross-model code review.

## Problem It Solves

Most AI agent failures aren't about model capability—they're about process:
- Starting to code before understanding the codebase
- Reinventing patterns that already exist in the repo
- Forgetting the original plan mid-implementation
- Missing edge cases that were obvious in hindsight

## Key Commands

| Command | What It Does |
| --- | --- |
| `/flow:plan` | Research + produce plan with acceptance checks |
| `/flow:work` | Execute plan end-to-end with task tracking |
| `/flow:interview` | Deep interview with 40+ questions before planning |
| `/flow:plan-review` | Carmack-level plan review via RepoPrompt |
| `/flow:impl-review` | Carmack-level implementation review |

## How It Works

**`/flow:plan`** runs 3 research agents in parallel:
- Gathers context before coding starts
- Identifies gaps and dependencies
- Writes plan with clear acceptance checks
- Optionally reviews via different model

**`/flow:work`** follows disciplined execution:
- Re-reads plan before each task
- Implements following existing patterns
- Runs tests automatically
- Ships with clear Definition of Done

## Features

- **Parallel Research** - 3 agents gather context simultaneously
- **Pattern Recognition** - Identifies and reuses existing code patterns
- **Plan-Driven Execution** - Re-reads plan between every task
- **Cross-Model Review** - External model review via RepoPrompt
- **Export Mode** - Export full context to paste into ChatGPT Pro, Claude web
- **Beads Integration** - Auto-detects and works with Beads task management
- **RepoPrompt Integration** - Token-efficient codebase exploration

## Installation

```bash
/plugin marketplace add https://github.com/gmickel/gmickel-claude-marketplace
/plugin install flow
```

## Usage Pattern

```bash
/flow:interview              # Optional: deep-dive before planning
/flow:plan "Feature description"  # Research + produce plan
/flow:work plans/slug.md     # Execute → test → ship
```

## Recent Updates

- **v0.7.7** - RepoPrompt v1.5.61 integration with prompt export capability
- **v0.7.4** - `/flow:interview` for 40+ question deep-dive
- **v0.7.0** - Export mode for external LLM review
- **v0.7.3** - Codex CLI support

## Technical Details

- **Repository:** gmickel/gmickel-claude-marketplace
- **Author:** Gordon Mickel
- **Language:** Shell/Markdown-based workflow
- **Stars:** 28+
- **Plugin Type:** Claude Code Marketplace

## Related Tools

- **RepoPrompt** - Token-efficient codebase exploration + cross-model reviews
- **Beads** - Dependency-aware issue tracking (auto-detected)
- **GNO** - Local hybrid search for notes, docs, and code

## Links

- [GitHub Repository](https://github.com/gmickel/gmickel-claude-marketplace)
- [Flow Documentation](https://github.com/gmickel/gmickel-claude-marketplace/tree/main/plugins/flow)
- [Author: Gordon Mickel](https://mickel.tech)
- [Original Tweet](https://x.com/gmickel/status/2007251220348682538)
