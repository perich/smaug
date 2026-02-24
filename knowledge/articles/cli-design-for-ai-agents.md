---
title: "CLI Design for AI Agents"
type: article
date_added: 2026-02-19
source: "https://joelclaw.com/cli-design-for-ai-agents"
author: "Joel Hooks"
tags: [cli-design, ai-agents, interfaces, json, hateoas]
via: "Twitter bookmark from @joelhooks"
---

A guide to designing command-line interfaces specifically for AI agents to parse and interact with, using machine-readable formats instead of human-friendly output formatting.

## Key Takeaways

- AI agents interact with tools primarily through stdout, not chat windows
- CLIs should return JSON envelopes for agent parsing instead of pretty tables
- HATEOAS navigation and NDJSON streaming enable agents to understand available actions
- Well-designed CLIs for agents also work well for humans through piping and jq

## Links

- [Article](https://joelclaw.com/cli-design-for-ai-agents)
- [Original Tweet](https://x.com/joelhooks/status/2024533555993596084)
