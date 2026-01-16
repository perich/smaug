---
title: "agent-browser"
type: tool
date_added: 2026-01-16
source: "https://github.com/vercel-labs/agent-browser"
tags: [browser-automation, ai-agents, cli-tools, headless-browser, web-scraping, typescript]
via: "Twitter bookmark from @jasonzhou1993"
---

agent-browser is a headless browser automation CLI tool designed for AI agents. It provides fast Rust CLI with a Node.js fallback, enabling agents to programmatically control and interact with web browsers from the command line.

Built by Vercel Labs, it has gained significant traction (6,800+ stars) as a lightweight, agent-friendly alternative to traditional browser automation libraries. The tool is particularly notable for its minimal context window overhead and ability to integrate with AI agents like Claude Code.

## Installation

### npm (recommended)
```bash
npm install -g agent-browser
agent-browser install  # Download Chromium
```

### From Source
```bash
git clone https://github.com/vercel-labs/agent-browser
cd agent-browser
pnpm install
pnpm build
pnpm build:native   # Requires Rust (https://rustup.rs)
pnpm link --global
agent-browser install
```

### Linux Dependencies
```bash
agent-browser install --with-deps
# or manually: npx playwright install-deps chromium
```

## Quick Start

```bash
agent-browser open example.com
agent-browser snapshot                    # Get accessibility tree with refs
agent-browser click @e2                   # Click by ref from snapshot
agent-browser fill @e3 "test@example.com" # Fill by ref
agent-browser get text @e1                # Get text by ref
agent-browser screenshot page.png
agent-browser close
```

## Core Commands

- **Navigation:** `open`, `goto`, `navigate`
- **Interaction:** `click`, `dblclick`, `focus`, `type`, `fill`, `press`, `keydown`, `keyup`, `hover`, `select`, `check`, `uncheck`
- **Scrolling:** `scroll`, `scrollintoview`, `scrollinto`
- **Advanced:** `drag`, `upload`, `eval`, `pdf`
- **Info Retrieval:** `get text`, `get html`, `get value`, `get attr`, `get title`, `get url`, `get count`, `get box`
- **State Checking:** `is visible`, `is enabled`, `is checked`

## Semantic Locators

Find elements by meaningful attributes rather than fragile selectors:

```bash
agent-browser find role button click --name "Submit"
agent-browser find text "Sign In" click
agent-browser find label "Email" fill "test@test.com"
agent-browser find first ".item" click
agent-browser find nth 2 "a" text
agent-browser find placeholder "Search" fill "query"
agent-browser find testid "submit-btn" click
```

## Wait Conditions

```bash
agent-browser wait <selector>         # Wait for element visibility
agent-browser wait <ms>               # Wait for time (milliseconds)
agent-browser wait --text "Welcome"   # Wait for text to appear
agent-browser wait --url "**/dash"    # Wait for URL pattern
agent-browser wait --load networkidle # Wait for load state
agent-browser wait --fn "window.ready === true"  # Wait for JS condition
```

## Key Features

- **Accessibility Tree Integration** - `snapshot` command provides semantic references for AI agents
- **Token Efficient** - Minimal context window overhead (95 tokens for instructions)
- **Ref-Based Selectors** - Use @e2, @e3 references instead of complex CSS selectors
- **Fallback Support** - Pure Node.js implementation if Rust CLI unavailable
- **Cross-Platform** - Works on Linux, macOS, and Windows
- **JavaScript Evaluation** - Run arbitrary JS with `eval` command
- **Load State Detection** - Wait for specific network/DOM states

## Integration with AI Agents

agent-browser is specifically designed for seamless integration with AI agents:

- Minimal token overhead allows more context for agent reasoning
- Accessibility tree snapshot provides semantic structure for agents to understand pages
- Simple ref-based commands are natural for AI to generate
- No setup required - works from any directory
- Can be triggered from Slack, GitHub, or browser contexts

## Performance

According to benchmarks shared by Jason Zhou (@jasonzhou1993):
- Instructions: only 95 tokens (~0.05% of context window)
- Same prompts consume 70% less tokens compared to traditional approaches
- Fast startup and execution suitable for rapid iteration

## Use Cases

- Web scraping for data extraction
- Form filling and automation
- UI testing and verification
- Screenshot capture and PDF generation
- Monitoring and health checks
- RPA (Robotic Process Automation)
- AI agent workflows and automation

## Language

TypeScript (with Rust CLI component)

## Related Tools

- Playwright - Traditional browser automation library
- Puppeteer - Chrome DevTools Protocol browser automation
- Selenium - Classic cross-browser automation
- Claude Code - AI coding agent that can use agent-browser

## Links

- [GitHub Repository](https://github.com/vercel-labs/agent-browser)
- [NPM Package](https://www.npmjs.com/package/agent-browser)
- [Related: Claude Code Documentation](https://code.claude.com/docs/)
