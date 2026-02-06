# Destructive Command Guard (dcg)

A high-performance hook for AI coding agents that blocks destructive commands before they execute, protecting your work from accidental deletion.

**Repository:** https://github.com/Dicklesworthstone/destructive_command_guard
**Language:** Rust
**License:** MIT
**Stars:** 340+

## Overview

dcg is designed to solve a critical problem: AI coding agents (Claude, GPT, etc.) occasionally run catastrophic commands like `git reset --hard`, `rm -rf ./src`, or `DROP TABLE users`—destroying hours of uncommitted work in seconds.

## Key Features

- **Zero-Config Protection**: Blocks dangerous git/filesystem commands out of the box
- **49+ Security Packs**: Databases (PostgreSQL, MySQL), Kubernetes, Docker, AWS/GCP/Azure, Terraform, and more
- **Sub-Millisecond Latency**: SIMD-accelerated filtering with Rust performance
- **Heredoc/Inline Script Scanning**: Catches embedded `python -c "os.remove(...)"` and shell scripts
- **Smart Context Detection**: Won't block `grep "rm -rf"` (data) but will block `rm -rf /` (execution)
- **Scan Mode for CI**: Pre-commit hooks and CI integration for code review
- **Fail-Open Design**: Never blocks workflow due to timeouts or parse errors
- **Explain Mode**: `dcg explain "command"` shows exactly why something is blocked
- **Agent-Friendly**: Explains why commands are blocked and suggests safe alternatives

## Technical Design

dcg balances several competing goals:

1. **Performance**: Must run for every tool call with sub-millisecond latency
2. **Avoiding False Positives**: Reduces friction without unnecessary agent waiting
3. **Resilience**: Uses AST-grep powered layer for heredoc/script detection, SIMD-optimized regex elsewhere
4. **Semantic Knowledge**: Expandable with domain-specific understanding (e.g., S3 bucket operations)
5. **Agent Integration**: Designed to work with Claude Code, Gemini CLI, OpenCode, Aider, Continue, and Codex CLI

## Supported Agents

- Claude Code
- Gemini CLI
- OpenCode (via community plugin)
- Aider (limited—git hooks only)
- Continue (detection only)
- Codex CLI (detection only)

## Quick Install

```bash
curl -fsSL "https://raw.githubusercontent.com/Dicklesworthstone/destructive_command_guard/master/install.sh?$(date +%s)" | bash -s -- --easy-mode
```

Works on Linux, macOS, and Windows (WSL). Auto-detects your platform and downloads the right binary.

## Usage Example

When an agent tries to run a dangerous command:

```bash
$ git reset --hard HEAD~5

════════════════════════════════════════════════════════════════
BLOCKED  dcg
────────────────────────────────────────────────────────────────
Reason:  git reset --hard destroys uncommitted changes

Command: git reset --hard HEAD~5

Tip: Consider using 'git stash' first to save your changes.
════════════════════════════════════════════════════════════════
```

## Configuration

Enable specific security packs based on your tech stack:

```toml
# ~/.config/dcg/config.toml
[packs]
enabled = [
    "database.postgresql",    # Blocks DROP TABLE, TRUNCATE
    "kubernetes.kubectl",     # Blocks kubectl delete namespace
    "cloud.aws",              # Blocks aws ec2 terminate-instances
    "containers.docker",      # Blocks docker system prune
]
```

## Agent-Specific Trust Levels

Configure different trust levels per agent:

```toml
[agents.claude-code]
trust_level = "high"
additional_allowlist = ["npm run build"]

[agents.unknown]
trust_level = "low"
extra_packs = ["paranoid"]
```

## Attribution

- **Jeffrey Emanuel**: Original concept and Python implementation, Rust expansion with modular pack system, heredoc scanning, three-tier architecture
- **Darin Gordon**: Initial Rust port with performance optimizations
- **Community**: Additional security packs and integrations
