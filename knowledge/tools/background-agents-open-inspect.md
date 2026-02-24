---
title: "Background Agents - Open-Inspect"
type: tool
date_added: 2026-02-10
source: "https://github.com/ColeMurray/background-agents"
tags: [agents, background-agents, ai-coding, development-infrastructure]
via: "Twitter bookmark from @_colemurray"
---

An open-source background agents coding system inspired by Ramp's Inspect. This is a hosted background coding agent that provides autonomous development capabilities with full environment access and multi-user collaboration support.

## Key Features

- Background task execution while developers focus on other work
- Full development environment access with all standard engineer tools
- Multiple client interfaces (web, Slack, Chrome extension)
- Multiplayer sessions for team collaboration
- Automatic PR creation with proper commit attribution
- Flexible AI model support (Anthropic Claude or OpenAI)
- Single-tenant deployment model with organization-level access control
- Shared GitHub App integration for seamless repository operations

## Architecture Highlights

- Cloudflare Durable Objects for control plane (state management, WebSocket hub, SQLite persistence)
- Modal platform for sandboxed session execution
- D1 database for repository-scoped secrets
- Supervisor/OpenCode/Bridge architecture in sandboxed VMs
- Support for full development environments (Git, package managers, databases, CI/CD)

## Links

- [GitHub](https://github.com/ColeMurray/background-agents)
- [Original Tweet](https://x.com/_colemurray/status/2021107964443230576)
