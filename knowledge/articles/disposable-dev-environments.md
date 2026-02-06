# Disposable Dev Environments with AI Safety Isolation

**Source:** https://jikkujose.in/2025/12/27/disposable-dev-environments.html

## Summary

A three-layer isolation architecture for safely running AI coding assistants (Claude Code, Aider, Copilot) by containing blast radius from compromised agents.

## Architecture Layers

### Layer 1: Host (macOS)
- Holds sensitive credentials (SSH keys, cloud tokens, API secrets)
- Runs only VM orchestration tools (kodemachine)
- No AI assistants execute here

### Layer 2: Virtual Machine (Linux)
- Provides development environment (editors, browsers, GUI apps)
- Can access network but not host filesystem
- Runs container management (testman)

### Layer 3: Container (Ephemeral)
- AI assistants execute in isolated containers
- Filesystem access limited to single mounted project directory
- Syscall logging via strace for audit trail
- Destroyed after each session

## Implementation Tools

| Tool | Function |
|------|----------|
| [kodemachine](https://github.com/jikkuatwork/kodemachine) | VM lifecycle management via UTM |
| [testman](https://github.com/jikkuatwork/testman) | Container orchestration via Podman |
| [dotfiles](https://github.com/jikkujose/dotfiles) | Consistent config across layers |

## Key Features

**VM Layer:**
- APFS copy-on-write cloning for instant VMs with zero disk overhead
- Headless operation enabling multiple concurrent instances
- QEMU guest agent for dynamic IP discovery

**Container Layer:**
- Ephemeral by default with `--rm` flag
- Project isolation (mounts single project directory)
- Syscall auditing via strace
- Pre-configured sandboxes for multiple AI assistants

## Threat Model

Context: Anthropic's November 2025 disclosure documented AI-enabled cyberattacks using Claude Code with 80-90% automation. This architecture assumes AI agents may be compromised and limits what they can access:

- Agent cannot access `~/.ssh`, `~/.aws`, or other projects
- Compromised agent's blast radius limited to one ephemeral container
- Credentials remain on host machine only

## Workflow

```bash
kodemachine start project    # Clone, boot, SSH in
testman run agentman ~/code/project  # Run AI in container
kodemachine suspend project  # Instant pause
kodemachine delete project   # Remove entirely
```

## Related Context

Connects to broader AI safety patterns:
- Defense in depth through layered isolation
- Ephemeral execution reducing state accumulation
- Syscall auditing for post-hoc analysis
- Credential isolation from execution environment
