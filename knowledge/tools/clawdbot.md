---
title: "Clawdbot"
type: tool
date_added: 2026-01-05
source: "https://github.com/steipete/clawdbot"
tags: [ai-agent, multi-surface, assistant, llm, automation, telegram, imessage, whatsapp]
via: "Twitter bookmarks from @moreconfetti, @doodlestein"
---

Clawdbot (formerly Clawdis) is a multi-surface AI assistant framework built by Peter Steinberger that brings Claude to multiple communication platforms simultaneously. It enables unified agentic workflows across web, Telegram, iMessage, WhatsApp, and voice interfaces.

Clawdbot represents a shift toward "inference-speed development" where AI agents can ship code and execute tasks autonomously while the developer sleeps or works on other problems. The framework is designed to be extensible through a skills system, allowing users to teach it new tools and integrations.

## Key Features

- **Multi-Surface Integration**: Works across Telegram, iMessage, WhatsApp, web, and voice
- **Skills System**: Markdown-based skill definitions teach the agent how to use CLI tools and integrations
- **Extensible Architecture**: Easy to add new integrations and tools through well-documented skill format
- **Context-Aware Execution**: Maintains conversation context and understands task completion criteria
- **Remote Access**: Can be accessed and controlled remotely through multiple messaging platforms

## Use Cases

- Autonomous coding and development tasks
- Personal AI assistant for email, messages, and notifications
- CI/CD and deployment automation via chat interfaces
- Interactive debugging and code exploration
- Multi-tool coordination and orchestration

## Integration with Other Tools

Clawdbot is designed to work with:
- **Agent Flywheel Tools**: Coordination layer for multi-agent development (cass, bv, ntm, agent-mail)
- **Cloud CLIs**: Wrangler (Cloudflare), Vercel, Supabase, Google Cloud
- **Development Tools**: GitHub, SSH, Cursor, tmux
- **Advanced Security**: ACIP (Advanced Cognitive Inoculation Prompt) for prompt injection protection

## Security Considerations

When deploying Clawdbot with sensitive tool access (emails, messaging, file systems), implementing ACIP is recommended to defend against prompt injection attacks and social engineering attempts.

## Links

- [GitHub Repository](https://github.com/steipete/clawdbot)
- [Shipping at Inference-Speed Article](https://steipete.me/posts/2025/shipping-at-inference-speed)
- [Agent Flywheel Skills Integration](https://github.com/Dicklesworthstone/agent_flywheel_clawdbot_skills_and_integrations)
- [Original Tweet](https://x.com/moreconfetti/status/2007866137191805130)
