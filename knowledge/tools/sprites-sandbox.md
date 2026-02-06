# Sprites: Stateful Sandbox Environments

**Website:** https://sprites.dev/
**Status:** Active service

## Overview
Sprites is a platform providing hardware-isolated execution environments (called "Sprites") for arbitrary code execution. A Sprite is a persistent Linux computer designed to safely run code blobs, AI agents (like Claude Code), or user-uploaded binaries.

## Key Features

### Checkpoint & Restore
- Save and restore the state of a sandbox environment at any point
- Enable reproducible testing and debugging workflows
- Allow rollback to known-good states

### Hardware Isolation
- Each Sprite is hardware-isolated from others
- Provides security and resource guarantees
- Suitable for executing untrusted code

### Persistent Linux Computers
- Full Linux environment within each Sprite
- Long-running applications supported
- Containerization-friendly

## Use Cases
- AI agent deployment and execution (e.g., Claude Code)
- Secure binary execution and analysis
- Development and testing environments
- Reproducible computation workflows
- Safe execution of user-uploaded code

## Benefits Over Alternatives
- Simpler than managing local infrastructure
- More flexible than cloud VPS (persistent state management)
- Better isolation than containerization alone
- Suitable for agents and autonomous workflows

## Integration
- Sign in via Fly.io OAuth integration
- API-driven execution model
- Support for session management and tracking
