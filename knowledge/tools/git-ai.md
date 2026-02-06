# git-ai - AI Code Attribution Tool

**GitHub:** https://github.com/git-ai-project/git-ai
**Stars:** 947
**Language:** Rust

## Overview
A vendor-agnostic Git extension for tracking AI-generated code in repositories. Records which coding agent, AI model, and prompt generated each line of code, with attribution surviving through git operations like merge, rebase, and cherry-pick.

## Key Features
- **Multi-agent support:** Works with Claude Code, Cursor, Copilot, GitHub Copilot, Google Gemini, and more
- **Accurate attribution:** Tracks code from generation through pull requests to merged commits
- **Git-native:** Built on git plumbing commands with negligible performance impact (<100ms even in large repos)
- **Workflow preservation:** AI-authorship annotations survive rebases, merges, squashes, cherry-picks
- **Prompt storage:** Maintains link between prompts and generated code

## Installation
```bash
# Mac, Linux, Windows (WSL)
curl -sSL https://usegitai.com/install.sh | bash

# Windows (non-WSL)
powershell -NoProfile -ExecutionPolicy Bypass -Command "irm http://usegitai.com/install.ps1 | iex"
```

## Supported Agents
- ✅ Cursor (>1.7)
- ✅ Claude Code
- ✅ GitHub Copilot in VSCode, Jetbrains IDEs
- ✅ Google Gemini CLI
- ✅ Continue CLI
- ✅ OpenCode
- ✅ Droid CLI (Factory AI)
- ✅ Atlassian RovoDev CLI

## How It Works
1. Coding agents call git-ai to mark lines as AI-generated
2. On commit, git-ai saves AI-attributions into Git Notes
3. CLI preserves notes through rebases, merges, squashes, cherry-picks
4. Powers AI-Blame view, AI contribution stats, and more

## Key Goals
- **Track AI code in multi-agent world:** Vendor-agnostic approach for diverse tool adoption
- **Accurate attribution:** Follow code through entire workflow from laptop to production
- **Support real-world git workflows:** Work with actual developer patterns
- **Maintain prompt context:** Keep requirements alongside code
- **Performance:** Git-native and fast, tested at Chromium-scale

## Use Cases
- Engineering team visibility into AI-assisted development
- Audit trail for AI-generated code compliance
- Understanding which prompts generated problematic code
- AI contribution metrics and team analytics
