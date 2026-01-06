---
title: "Agent Flywheel Clawdbot Skills & Integrations"
type: tool
date_added: 2026-01-05
source: "https://github.com/Dicklesworthstone/agent_flywheel_clawdbot_skills_and_integrations"
tags: [clawdbot, skills, integrations, agentic-coding, acfs, cli-tools]
via: "Twitter bookmark from @doodlestein"
---

Agent Flywheel Clawdbot Skills & Integrations is a curated collection of Clawdbot skills for professional agentic coding workflows. It brings together tools from the Agent Coding Flywheel Setup (ACFS) ecosystem with popular cloud and development infrastructure CLIs, all packaged as reusable Clawdbot skills.

Skills are markdown files that teach Clawdbot how to use command-line tools effectively. When enabled, Clawdbot can intelligently use these tools across WhatsApp, Telegram, iMessage, web, and voice interfaces.

## What Are Clawdbot Skills?

Skills are markdown documentation files that contain:
- Tool description and purpose
- Command syntax and examples
- Best practices and common workflows
- Expected output patterns and error handling

## Included Skills Categories

### Dicklesworthstone Stack (Agentic Coding Tools)
- **ntm** (Named Tmux Manager): Orchestrate Claude Code, Codex, and Gemini in tiled tmux panes
- **agent-mail**: MCP Agent Mail coordination layer with mailboxes and file reservations
- **bv** (Beads Viewer): TUI for task management with dependency graphs
- **cass** (Coding Agent Session Search): Unified history from all AI coding agents
- **cm**: CASS Memory System with procedural memory and rule playbook
- **slb** (Simultaneous Launch Button): Two-person rule enforcement for dangerous commands

### Cloud & Infrastructure
- **gcloud**: Google Cloud Platform (Compute, Cloud Run, GKE, Storage, BigQuery)
- **wrangler**: Cloudflare Workers, KV, R2, D1, Pages
- **vercel**: Vercel deployments, domains, environment variables
- **supabase**: Supabase DB, migrations, Edge Functions, storage

### Browser Automation
- **claude-chrome**: Control authenticated browser, automate workflows, fill forms, extract data

### Media & Image Tools
- **giil** (Get Image from Internet Link): Download full-resolution images from iCloud, Dropbox, Google Photos, Google Drive share links

### Documentation & Export
- **csctf** (Chat Shared Conversation To File): Convert ChatGPT, Gemini, Grok, Claude share links to clean Markdown + HTML transcripts

### Development Tools
- **github**: GitHub CLI for repos, issues, PRs, Actions, releases
- **ssh**: SSH patterns, tunnels, keys, rsync
- **cursor**: Cursor AI editor CLI
- **ghostty**: Ghostty terminal emulator control
- **wezterm**: WezTerm terminal multiplexer

## Installation

### One-Line Install (Recommended)

Install all skills:
```bash
curl -fsSL "https://raw.githubusercontent.com/Dicklesworthstone/agent_flywheel_clawdbot_skills_and_integrations/main/install.sh?v=$(date +%s)" | bash -s -- --all
```

Or pick skills interactively:
```bash
curl -fsSL "https://raw.githubusercontent.com/Dicklesworthstone/agent_flywheel_clawdbot_skills_and_integrations/main/install.sh?v=$(date +%s)" | bash
```

The installer automatically:
- Detects your Clawdbot skills directory
- Shows categorized menu for skill selection
- Generates config snippet for clawdbot.json

## Key Features

- **Modular Design**: Install only the skills you need
- **Auto-Detection**: Works with standard Clawdbot installation paths
- **Easy Integration**: Generated config snippets for seamless Clawdbot integration
- **Comprehensive Tooling**: Covers entire agentic development workflow from coding to deployment

## Use Cases

- **Professional Agentic Coding**: Manage multi-agent development sessions with ntm and cass
- **Cloud Deployment**: Deploy to GCP, Cloudflare, Vercel, or Supabase through Clawdbot
- **Workflow Automation**: Automate complex workflows across multiple tools
- **Browser Automation**: Control authenticated browser sessions for data extraction or form filling
- **Multi-Agent Coordination**: Coordinate multiple Claude Code instances with task management

## How It Differs from Standard Clawdbot

While Clawdbot comes with basic integrations, this collection:
- Adds specialized agentic coding tools (ntm, cass, bv)
- Includes comprehensive cloud infrastructure support
- Provides browser automation capabilities
- Offers media download and document conversion tools
- Curates best practices for each tool in skill documentation

## Links

- [GitHub Repository](https://github.com/Dicklesworthstone/agent_flywheel_clawdbot_skills_and_integrations)
- [Agentic Coding Flywheel Setup](https://github.com/Dicklesworthstone/agentic_coding_flywheel_setup)
- [Original Tweet](https://x.com/doodlestein/status/2007996215892336924)
- [Clawdbot Project](https://github.com/steipete/clawdbot)
