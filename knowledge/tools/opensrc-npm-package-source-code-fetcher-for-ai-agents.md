---
title: "opensrc: npm Package Source Code Fetcher for AI Agents"
type: tool
date_added: 2026-02-15
source: "https://github.com/vercel-labs/opensrc"
tags: [npm, ai-agents, source-code, typescript, developer-tools, coding-agents]
via: "Twitter bookmark from @jachands"
---

CLI tool that fetches source code for npm packages to give AI coding agents deeper context than types and documentation alone. When working with AI agents, understanding implementation details is crucial—opensrc automates the process of fetching and organizing package source code.

## Key Features

- Fetch source code for npm packages with version auto-detection from lockfiles
- Support for multiple package managers (package-lock.json, pnpm-lock.yaml, yarn.lock)
- Direct GitHub repository support (owner/repo syntax, URLs, branches/tags)
- Batch fetching of multiple packages and repos
- Automatic file modifications (optional):
  - Updates .gitignore with opensrc/ directory
  - Excludes opensrc/ from tsconfig.json
  - Adds AGENTS.md section for agent reference
- Global source code cache with automatic updates
- CLI commands: list, remove, and re-fetch sources

## Usage Examples

```bash
# npm packages
opensrc zod
opensrc zod@3.22.0
opensrc react react-dom next

# GitHub repositories
opensrc github:owner/repo
opensrc facebook/react
opensrc https://github.com/colinhacks/zod
opensrc owner/repo@v1.0.0

# Management
opensrc list
opensrc remove zod
```

## Links

- [GitHub](https://github.com/vercel-labs/opensrc)
- [Original Tweet](https://x.com/jachands/status/2023006669324857445)
