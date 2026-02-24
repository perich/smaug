---
title: "Zerobrew - Fast Homebrew Alternative"
type: tool
date_added: 2026-02-10
source: "https://github.com/lucasgelfond/zerobrew"
tags: [package-manager, homebrew, macos, rust, cli, performance]
via: "Twitter bookmark from @orhundev"
---

Zerobrew is a modern Rust-based drop-in replacement for Homebrew on macOS that achieves 5-20x faster performance through content-addressable storage and parallel downloads. It's an experimental but increasingly practical alternative that maintains compatibility with Homebrew's formula ecosystem.

## Key Features

- Content-addressable store with deduplication for efficient storage
- Parallel downloads for faster installation
- APFS clonefile support for zero-overhead file copying
- Fallback to source builds using Homebrew's Ruby DSL
- Full compatibility with Homebrew's formula definitions and metadata
- Dual-licensed (MIT or Apache 2.0)
- Support for Brewfile (bundle management)
- Pre-built bottle support from Homebrew infrastructure

## Performance

Demonstrates significant speedups across various packages:
- Overall top 100 packages: 2.0x cold, 7.6x warm speedup
- Libsodium: 6.0x cold, 18.1x warm
- SQLite: 4.6x cold, 18.1x warm
- Tesseract: 3.4x cold, 29.5x warm

## Usage

```bash
zb install jq                    # install one package
zb install wget git              # install multiple
zb bundle                        # install from Brewfile
zb uninstall jq                  # uninstall package
zb reset                         # uninstall everything
zbx jq --version                 # run without linking
```

## Links

- [GitHub](https://github.com/lucasgelfond/zerobrew)
- [Original Tweet](https://x.com/orhundev/status/2021301890827550970)
