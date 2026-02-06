# Claude Code Documentation Mirror

A local mirror of Claude Code documentation that can be accessed faster than fetching from the web. Maintained by Eric Buess.

## Key Features

- Automatic updates every 3 hours from official Anthropic documentation
- Local file access for faster documentation lookup
- Changelog integration for Claude Code release notes
- `/docs` slash command for easy access within Claude Code
- Cross-platform support (macOS and Linux)

## Installation

```bash
curl -fsSL https://raw.githubusercontent.com/ericbuess/claude-code-docs/main/install.sh | bash
```

## Usage

Basic usage with the `/docs` command:
- `/docs hooks` - Read hooks documentation instantly
- `/docs mcp` - Read MCP documentation
- `/docs changelog` - Read Claude Code release notes
- `/docs -t` - Check documentation sync status with GitHub

## Platform Support

- macOS (fully supported)
- Linux (Ubuntu, Debian, Fedora, etc.)
- Windows (not yet supported)

## Repository

[ericbuess/claude-code-docs](https://github.com/ericbuess/claude-code-docs) - 664 stars

Created by Eric Buess as a mirror of official Claude Code documentation at https://docs.anthropic.com/en/docs/claude-code/
