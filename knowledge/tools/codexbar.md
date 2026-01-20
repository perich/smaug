# CodexBar

## Overview
CodexBar is a macOS menu bar app that provides real-time visibility into API usage limits across multiple AI services. It helps developers track session and weekly usage to avoid hitting rate limits.

## Key Features
- **Multi-provider support**: Codex, Claude Code, Cursor, Gemini, Antigravity, Droid, Copilot, z.ai
- **Real-time usage tracking**: Displays session and weekly usage meters with reset countdowns
- **Credits tracking**: Shows optional credits and code review limits
- **Status monitoring**: Provider status polling with incident badges
- **WidgetKit support**: Menu card snapshot that mirrors the app display
- **CLI tool**: Bundled `codexbar` CLI for scripts and CI
- **Minimal UI**: No Dock icon, clean menu bar integration

## Architecture
- **Cookies-based**: Reuses existing browser cookies (Safari/Chrome/Firefox) for dashboard access
- **No passwords stored**: Privacy-focused approach
- **Two-bar icon**: Session usage on top, weekly on bottom
- **Dimmed on errors**: Visual feedback for connection issues

## Installation
- Download from GitHub Releases
- Homebrew: `brew install --cask steipete/tap/codexbar`
- Available for macOS 14+ (Apple Silicon + Intel)
- Sparkle updates enabled on GitHub builds only

## Permissions
- Full Disk Access: Only for Safari cookies
- Keychain access: For token storage
- Files & Folders: When provider CLIs access project directories

## Repository
https://github.com/steipete/CodexBar

## Links
- [Website](https://codexbar.app/)
- [GitHub Releases](https://github.com/steipete/CodexBar/releases/latest)
- [Provider Documentation](https://github.com/steipete/CodexBar/blob/main/docs/providers.md)
- [CLI Documentation](https://github.com/steipete/CodexBar/blob/main/docs/cli.md)
- [Provider Guide](https://github.com/steipete/CodexBar/blob/main/docs/provider.md)

## Creator
Built by [Peter Steinberger](https://steipete.me) ([steipete](https://x.com/steipete))
