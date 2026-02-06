# Codex Skill Manager

macOS SwiftUI app for managing Codex and Claude Code skills.

- **Repository:** https://github.com/Dimillian/CodexSkillManager
- **Language:** Swift
- **Stars:** 805
- **Platform:** macOS 26+ with Swift 6.2+

## Features
- Browse local skills from ~/.codex/skills, ~/.codex/skills/public, and ~/.claude/skills
- Render SKILL.md with Markdown and inline reference previews
- Import skills from folders or zip files
- Delete skills from sidebar
- Browse Clawdhub skills with search and latest drops
- Download remote skills into Codex or Claude Code
- Visual tags for installed status and versions

## Building
```bash
swift build
swift run CodexSkillManager
```

## Packaging
```bash
./Scripts/compile_and_run.sh
```

## Dependencies
- Markdown rendering via swift-markdown-ui
- Remote skill catalog via Clawdhub

## Use Case
Manage and discover AI agent skills with a native macOS interface.

## Link
- https://github.com/Dimillian/CodexSkillManager
