---
title: "Spacebot - Rust-based AI Agent for Teams and Communities"
type: tool
date_added: 2026-02-17
source: "https://github.com/spacedriveapp/spacebot"
tags: [ai-agent, rust, team-collaboration, discord, slack, async-architecture]
via: "Twitter bookmark from @jamiepine"
---

A Rust-based agentic operating system designed for large Slack and Discord communities. Spacebot solves the fundamental problem with existing AI frameworks where a single session handles conversation, thinking, and task execution sequentially—meaning the agent goes silent while working.

Spacebot's architecture separates concerns: the conversation layer never touches tools directly. Instead, it delegates thinking to branches and heavy tasks to workers, enabling truly concurrent responses. Even with 100 people talking simultaneously, the system remains responsive and never blocks.

## Key Features

- **Concurrent Architecture** - Branches handle thinking while workers execute tasks, allowing responsive conversations regardless of load
- **Automated Memory Management** - Automatically transforms memory files, notes, documents, and chat histories into structured memories with 8 typed categories, graph associations, and hybrid search
- **Built-in Developer Tools** - OpenCode workers for deep coding sessions, browser automation, Brave web search, cron jobs, and OpenClaw-compatible skill system
- **Control UI** - Gorgeous interface for monitoring and managing the system
- **Cortex Oversight** - Central system that audits memories, actions goals and todos
- **Flexible Deployment** - Self-host as a single Rust binary or use one-click cloud deploy
- **Multi-agent Support** - Run multiple agents on one instance with different identities, memories, and security permissions
- **Message Coalescing** - Detects rapid-fire message bursts, batches them intelligently, and lets the LLM decide what to engage with

## Links

- [GitHub](https://github.com/spacedriveapp/spacebot)
- [Website](https://spacebot.sh)
- [Original Tweet](https://x.com/jamiepine/status/2023631346434798060)
