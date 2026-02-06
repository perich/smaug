# Post-Compact Reminder for Claude Code

**Repository:** https://github.com/Dicklesworthstone/post_compact_reminder
**Language:** Shell
**Stars:** 14

## Summary
A Claude Code hook tool that reminds Claude agents to re-read AGENTS.md after context compaction to prevent loss of project conventions during long coding sessions.

## Problem It Solves
When Claude Code compacts conversation history to stay within context limits, the agent loses memory of the AGENTS.md file that defines coding conventions, forbidden commands, architectural decisions, and multi-agent coordination rules. This causes Claude to ignore project rules and act unpredictably after compaction.

## How It Works
The tool uses a workaround mechanism due to a bug in Claude Code's SessionStart hook with compact matcher:

1. **PreCompact hook** - Writes a marker file when compaction is about to happen
2. **UserPromptSubmit hook** - Checks for the marker on the next user message
3. **Reminder injection** - If marker exists, injects the reminder into Claude's context and deletes the marker

This ensures the reminder appears on the first message after compaction when Claude needs it most.

## Installation
```bash
curl -fsSL https://github.com/Dicklesworthstone/post_compact_reminder/raw/refs/heads/main/install-post-compact-reminder-workaround.sh | bash
```

Or check health:
```bash
./install-post-compact-reminder-workaround.sh --status
```

## Key Features
- **Automatic detection** - Fires only after compaction, not on normal startups
- **Zero-config** - Installs globally in `~/.local/bin` and `~/.claude/settings.json`
- **Customizable messages** - 4 built-in templates (minimal, detailed, checklist, default) plus custom options
- **Reliable injection** - Workaround mechanism ensures Claude actually sees the reminder
- **Idempotent installer** - Safe to run repeatedly; creates backups automatically
- **Self-updating** - Use `--update` flag to pull latest version from GitHub

## Related
- Claude Code agents and multi-agent coordination
- Context management and compaction strategies
- Hook systems for Claude Code customization
