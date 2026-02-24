---
title: "React Doctor - Code Analysis Tool"
type: tool
date_added: 2026-02-17
source: "https://github.com/millionco/react-doctor"
tags: [react, code-review, agents, quality-assurance]
via: "Twitter bookmark from @aidenybai"
---

React Doctor is a CLI tool that analyzes React codebases for anti-patterns, performance issues, and architectural problems. It scans for issues like unnecessary useEffects, accessibility problems, prop drilling, and provides a 0-100 health score to guide improvements.

## Key Features

- Dual-pass analysis: Lint checks (60+ rules) and dead code detection
- Supports multiple frameworks: Next.js, Vite, Remix, and more
- Automatic framework and React version detection
- Severity-based scoring system (75+ Great, 50-74 Needs work, <50 Critical)
- Integrates with CI/CD via GitHub Actions
- Installable as a coding agent skill
- Configuration via react-doctor.config.json or package.json
- Verbose mode to see affected files and line numbers

## Links

- [GitHub](https://github.com/millionco/react-doctor)
- [Original Tweet](https://x.com/aidenybai/status/2023806826580766793)
