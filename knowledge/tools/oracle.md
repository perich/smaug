---
title: "Oracle"
type: tool
date_added: 2026-01-11
source: "https://github.com/steipete/oracle"
tags: [ai-coding, claude-code, gpt-5-pro, multi-model, context-bundling, cli-tools, typescript]
via: "Twitter bookmark from @davidgasquez"
---

Oracle is a CLI tool that bundles your prompt and files so AI models can answer with real context. It supports multiple frontier models including GPT-5 Pro, Claude (Sonnet 4.5, Opus 4.1), and Gemini 3 Pro, with both API and browser automation modes.

Created by steipete, Oracle enables developers to send code context and custom prompts to multiple AI models in a single run, supporting both synchronous API calls and browser-based interactions. The tool handles file bundling, model selection, and response management, making it easy to leverage different models' strengths.

## Key Features

- **Multi-Model Support** - Works with GPT-5.1 Pro, GPT-5.2 Pro, Claude Sonnet 4.5, Claude Opus 4.1, Gemini 3 Pro, and more
- **Dual Engine Modes** - API mode for reliability, browser mode for ChatGPT web interface without API keys
- **File Bundling** - Automatically bundles selected files (with glob pattern support) as context
- **Flexible Output** - Copy-paste to ChatGPT, API response handling, or preview mode
- **Session Tracking** - Keeps history of runs and responses for replay/review
- **Interactive TUI** - Terminal UI mode for interactive exploration

## Installation

```bash
npm install -g @steipete/oracle
# or
brew install steipete/tap/oracle
```

Requires Node 22+. Can also use `npx -y @steipete/oracle` without installation.

## Common Usage Patterns

**API Mode (Recommended)**
```bash
# Single model review
npx -y @steipete/oracle -p "Review the TS data layer for schema drift" --file "src/**/*.ts,*/*.test.ts"

# Multi-model cross-check
npx -y @steipete/oracle -p "Cross-check the data layer assumptions" --models gpt-5.1-pro,gemini-3-pro --file "src/**/*.ts"
```

**Browser Mode (No API Key)**
```bash
# Browser-based ChatGPT interaction
npx -y @steipete/oracle --engine browser -p "Walk through the UI smoke test" --file "src/**/*.ts"

# Gemini browser mode with Chrome cookies
npx -y @steipete/oracle --engine browser --model gemini-3-pro --prompt "a cute robot holding a banana" --generate-image out.jpg
```

**Preview & Sessions**
```bash
# Dry-run preview without token spend
npx -y @steipete/oracle --dry-run summary -p "Check release notes" --file docs/release-notes.md

# View recent sessions
npx -y @steipete/oracle status --hours 72

# Replay a previous session
npx -y @steipete/oracle session <id> --render

# Interactive TUI mode
npx -y @steipete/oracle tui
```

## Configuration

- **API Keys** - Set `OPENAI_API_KEY`, `GEMINI_API_KEY`, `ANTHROPIC_API_KEY` in environment
- **ChatGPT Custom Project** - Use `browser.chatgptUrl` in config to keep browser runs organized
- **Remote Browser** - Run `oracle serve` on signed-in host; clients use `--remote-host/--remote-token`
- **MCP Integration** - Available as stdio server via `oracle-mcp` for Cursor/other MCP clients

## Engine-Specific Notes

- **API Mode** - Most reliable, requires valid API keys, predictable costs
- **Browser Mode (macOS)** - Stable implementation, auto-detects browser
- **Browser Mode (Linux)** - Works but may need `--browser-chrome-path/--browser-cookie-path` flags
- **Browser Mode (Windows)** - Recommend `--browser-manual-login` or inline cookies

## Use Cases

- **Code Review** - Send entire modules for architectural review
- **Bug Investigation** - Bundle error logs, traces, and relevant code together
- **Multi-Model Consensus** - Compare approaches across different frontier models
- **Documentation** - Generate architecture notes from codebase context
- **Integration Tests** - Have models review complex flows with actual code context

## Cost Considerations

- API mode costs depend on prompt/completion tokens and model selection
- GPT-5.2 Pro is expensive but capable; budget ~$7-10 per complex code review
- Browser mode has no API costs but is experimental and slower
- Session tracking helps review cost vs. benefit of different prompts

## Significance

Oracle solves a key workflow problem: how to leverage frontier models without manual copy-paste or context loss. By bundling files and prompts, it ensures models have sufficient context for meaningful analysis. The multi-model support allows teams to cross-check critical decisions across different AI providers' architectures.

## Links

- [GitHub Repository](https://github.com/steipete/oracle)
- [NPM Package](https://www.npmjs.com/package/@steipete/oracle)
- [Documentation](https://github.com/steipete/oracle/blob/main/README.md)
- [Original Tweet](https://x.com/davidgasquez/status/2010369069564690717)

