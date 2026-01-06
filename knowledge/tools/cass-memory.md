---
title: "cass-memory"
type: tool
date_added: 2026-01-05
source: "https://github.com/Dicklesworthstone/cass_memory_system"
tags: [ai-agents, memory-systems, procedural-memory, coding-agents, knowledge-management]
via: "Twitter bookmark from @doodlestein"
---

Procedural memory system for AI coding agents that transforms scattered agent sessions into persistent, cross-agent memory. Enables every agent to learn from every other agent's experience through a three-layer cognitive architecture: episodic (raw ground truth), working (structured summaries), and procedural (distilled rules with confidence tracking).

## Key Features

- **Cross-Agent Learning:** Sessions from all AI coding agents (Claude Code, Cursor, Codex, Aider, etc.) feed into a unified knowledge base
- **Three-Layer Architecture:** Episodic memory (cass search engine) → Working memory (diary entries) → Procedural memory (playbook with confidence tracking)
- **Automatic Consolidation:** Patterns discovered in one agent automatically help all other agents on subsequent sessions
- **MCP Server:** Model Context Protocol integration for seamless agent integration
- **ACE Pipeline:** Complete implementation of Generate → Reflect → Curate → Validate workflow
- **Confidence Tracking:** Rules decay and are updated based on validation feedback
- **Cross-Platform:** Runs on Linux, macOS, and Windows

## MVP Status

The core system reached ~85-90% complete with:
- 151 passing tests
- Compiled binary
- All core commands working
- ACE pipeline fully functional
- Remaining work focused on test coverage and polish

## Installation

```bash
curl -fsSL https://raw.githubusercontent.com/Dicklesworthstone/cass_memory_system/main/install.sh \
  | bash -s -- --easy-mode --verify
```

## Use Cases

- Build institutional memory across AI assistant tools
- Share debugging strategies and patterns between agents
- Maintain project-specific insights in persistent knowledge
- Create sophisticated multi-agent workflows with learning
- Team collaboration: patterns from any team member's AI assistant benefit everyone

## Links

- [GitHub](https://github.com/Dicklesworthstone/cass_memory_system)
- [Original Tweet](https://x.com/doodlestein/status/2008226781870854531)
- [Project Plan](https://github.com/Dicklesworthstone/cass_memory_system/blob/main/PLAN_FOR_CASS_MEMORY_SYSTEM.md)
- [Improvement Ideas](https://github.com/Dicklesworthstone/cass_memory_system/blob/main/SUGGESTED_IMPROVEMENTS_TO_CASS_BASED_ON_CMS.md)
