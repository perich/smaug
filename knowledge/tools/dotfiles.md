# Dotfiles - Development Environment Configuration

**Repository:** https://github.com/elithrar/dotfiles
**Stars:** 130
**Language:** TypeScript
**Description:** dotfiles & installation script for macOS & Linux development environments

## Overview

A comprehensive dotfiles repository for setting up a complete development environment on macOS and Linux, including configuration files, installation scripts, and tooling setup.

## Components

### Installation Script (`install.sh`)
Sets up dependencies, installs Homebrew and related packages, and links in dotfiles on macOS and Linux. Safe to run repeatedly (checks for existing installs).

### Dotfiles
Configuration files for shell, terminal, editor, and other development tools:
- `.tmux.conf` - Terminal multiplexer configuration
- `.zshrc` - Zsh shell configuration
- Editor configurations
- And more

## Installation

```bash
# Install dependencies and packages
sh install.sh 2>&1 | tee ~/install.log

# Use GNU Stow to symlink dotfiles
stow --dir="${HOME}/repos/dotfiles" --target="${HOME}" .
```

## What's Included

### Terminal & Shell
- **Ghostty** - Primary terminal environment on macOS (installed via install.sh)
- **zsh** - Shell environment
- **oh-my-zsh** - Zsh framework and plugins
- **tmux** - Terminal multiplexer with configuration

### Editor
- **Zed** - Primary editor (previously: VS Code)

### Font
- **Berkeley Mono** (TX-02) - Monospace font for coding

## Key Features

- WSL support (can be run in WSL on Windows)
- Safe and idempotent (checks for existing installations before updating)
- Inspired by [formation](https://github.com/minamarkham/formation)
- Comprehensive development environment setup

## Special Features for This Repository

The dotfiles include configuration for code review workflows:
- **OpenCode command-line configuration** at `.config/opencode/command/code-review.md`
- **OpenCode subagent configuration** at `.config/opencode/agent/code-review.md`
- Parallel code review agents with temperature 0.1 for improved quality
- Integration with development workflow

## Use Cases

- Quickly set up a new development machine
- Maintain consistent development environment across multiple machines
- Share development setup with team members
- Version control configuration as code

## License

See LICENSE file for details.
