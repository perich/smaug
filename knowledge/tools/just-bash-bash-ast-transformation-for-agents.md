---
title: "just-bash: Bash AST Transformation for Agents"
type: tool
date_added: 2026-02-14
source: "https://github.com/vercel-labs/just-bash"
tags: [bash, agents, ast, typescript, sandboxing]
via: "Twitter bookmark from @cramforce"
---

A TypeScript-based simulated bash environment with in-memory virtual filesystem, designed for AI agents that need a secure, sandboxed bash environment. The key innovation is its AST parsing and transformation capability—it can parse and re-serialize shell scripts without executing them.

## Key Features

- In-memory bash environment with virtual filesystem
- AST parsing and transformation of shell scripts without execution
- Optional network access with secure-by-default URL filtering
- Custom command definitions via TypeScript
- Multiple filesystem implementations (InMemoryFs, OverlayFs, ReadWriteFs)
- Vercel Sandbox compatible API
- Interactive shell support
- Execution protection against infinite loops and recursion
- Support for shell piping and I/O redirection

## Built-in Transformers

- **Auto-tee transformer:** Automatically pipes command output to files for later inspection without re-execution
- **Script auditing:** Generate trustable reports of commands in scripts for permission verification before execution

## Links

- [GitHub](https://github.com/vercel-labs/just-bash)
- [Original Tweet](https://x.com/cramforce/status/2022778424784490944)
