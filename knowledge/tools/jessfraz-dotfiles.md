# jessfraz/dotfiles - Developer Configuration Reference

Configuration files and build system for development environment setup.

**Repository:** https://github.com/jessfraz/dotfiles
**Language:** Shell
**Stars:** 3533
**Topics:** bash, containers, docker, dotfiles, linux, shell

## Overview

Jessie Frazelle's well-maintained dotfiles repository featuring battle-tested shell configurations, vim setup, and development environment tooling. The repository includes an AGENTS.md file that documents recommended tools and workflows.

## Installation

```bash
make
```

This creates symlinks from the repo to your home folder.

## Key Components

### AGENTS.md

The AGENTS.md file documents tools, workflows, and development practices that the maintainer relies on. This file serves as a reference for:

- Tools that are essential for daily development
- Workflows and best practices
- Configuration patterns for development environments
- Recommendations for other developers

### .vim

For vim configuration, this repo references a separate repo: [github.com/jessfraz/.vim](https://github.com/jessfraz/.vim)

### Customization

Save environment variables and secrets in a `.extra` file:

```bash
# .extra - not committed to repo
###
### Git credentials
###
GIT_AUTHOR_NAME="Your Name"
GIT_COMMITTER_NAME="$GIT_AUTHOR_NAME"
git config --global user.name "$GIT_AUTHOR_NAME"
GIT_AUTHOR_EMAIL="email@you.com"
GIT_COMMITTER_EMAIL="$GIT_AUTHOR_EMAIL"
git config --global user.email "$GIT_AUTHOR_EMAIL"
GH_USER="nickname"
git config --global github.user "$GH_USER"

###
### Gmail credentials for mutt
###
export GMAIL=email@you.com
export GMAIL_NAME="Your Name"
export GMAIL_FROM=from-email@you.com
```

## Testing

The repository includes tests using [shellcheck](https://github.com/koalaman/shellcheck) in a container:

```bash
make test
```

## Quality Assurance

- CI/CD via GitHub Actions for shell linting and validation
- Container-based testing for consistency
- Well-documented customization patterns

## Use Cases

- **Reference Implementation:** See how a highly experienced developer structures their dotfiles
- **Tool Discovery:** The AGENTS.md file highlights essential tools and workflows
- **Shell Configuration:** Learn bash and shell scripting patterns
- **Docker/Container Knowledge:** Excellent examples of containerized development setups

## Philosophy

The repository is described as "pretty ocd and pedantic" — highly organized and detail-oriented. This is a reference point for developers seeking to understand experienced approaches to environment setup and configuration management.

## Related Resources

- [jessfraz/.vim](https://github.com/jessfraz/.vim) - Separate vim configuration repo
- [Jessie Frazelle's Blog](https://blog.jessfraz.com/) - Additional context on development practices
