---
title: "API2CLI - Generate CLIs from API documentation"
type: tool
date_added: 2026-02-20
source: "https://github.com/alexknowshtml/api2cli"
tags: [claude-code, skill, api, cli-generator, commander-js, nodejs, typescript]
via: "Twitter bookmark from @alexhillman"
---

A Claude Code skill that automatically transforms API documentation into fully functional dual-mode CLIs using Commander.js. Discovers endpoints from API docs, generates complete CLI implementations, and creates reusable agent skills.

## Key Features

- Discovers endpoints from API documentation, live URLs, or network captures
- Generates Commander.js CLIs with one subcommand per endpoint
- Dual-mode output: human-readable in terminal, JSON with suggestions when piped
- Automatic authentication, pagination, and rate limiting handling
- Full API client with error handling and retry logic
- Generates SKILL.md files for future Claude sessions to use the CLI
- Support for multiple API styles and complex authentication schemes

## How It Works

1. Point api2cli at API documentation or live endpoint
2. Claude discovers available endpoints and builds endpoint catalog
3. Generates a complete CLI with all endpoints as subcommands
4. Creates a reusable skill so other Claude sessions can use it without reading code
5. Dual-mode output automatically detects terminal vs piped usage

## Example: Resend Email API

```bash
# Generate CLI
Build me a CLI for the Resend API. Here are the docs: https://resend.com/docs/api-reference

# Use generated CLI
resend emails send --to user@example.com --subject "Hello"
resend domains list
resend contacts create --email user@example.com
```

## Links

- [GitHub](https://github.com/alexknowshtml/api2cli)
- [Original Tweet](https://x.com/alexhillman/status/2024651709503483944)
