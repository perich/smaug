# Warden - AI Code Review Agents

**URL:** https://warden.sentry.dev/

Warden is a Sentry tool that provides agents for reviewing your code either locally or on every PR. It's built to integrate with development workflows to catch issues automatically.

## Key Features
- Local code review capability
- GitHub PR integration
- Built on Claude AI agents for intelligent code analysis
- Configuration via `warden.toml`
- GitHub Actions workflow support

## Installation
Available via npm, pnpm, or bun:
```
npm install -g @sentry/warden
```

## Getting Started
1. Install the CLI globally
2. Initialize project: `warden init`
3. Add a skill: `warden add <skill-name>`
4. Set `WARDEN_ANTHROPIC_API_KEY` in .env.local
5. Add the key to repository secrets
6. Commit and open a PR to test

## Reference
- Mentioned by: @zeeg (David Cramer, Sentry)
- Status: Early stage, demo/writeup coming soon
