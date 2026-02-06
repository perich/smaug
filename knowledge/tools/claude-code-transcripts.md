# claude-code-transcripts

**Repository:** https://github.com/simonw/claude-code-transcripts

**Description:** Tools for publishing transcripts for Claude Code sessions

**Language:** Python

**Stars:** 962

## Overview

Convert Claude Code session files (JSON or JSONL) to clean, mobile-friendly HTML pages with pagination.

## Key Features

- Interactive session picker for local Claude Code sessions
- Web sessions import via Claude API
- Multiple output options and formatting
- GitHub Gist integration for sharing
- Auto-naming and pagination support

## Commands

- `local` - select from local sessions stored in `~/.claude/projects`
- `web` - select from web sessions via Claude API
- `json` - convert a specific JSON or JSONL file
- `all` - convert all local sessions to browsable HTML archive

## Installation

```bash
uv tool install claude-code-transcripts
# or run without installing:
uvx claude-code-transcripts --help
```

## Usage

Quick start to view a recent session:

```bash
claude-code-transcripts
```

Output options:
- `-o, --output DIRECTORY` - specify output directory
- `-a, --output-auto` - auto-name output subdirectory based on session ID
- `--repo OWNER/NAME` - GitHub repo for commit links
- `--open` - open generated HTML in browser (default)
- `--gist` - upload to GitHub Gist
- `--json` - include original session file in output

## Mentioned By

- @mtrajan discussing MCP analytics and Claude Code extensions
