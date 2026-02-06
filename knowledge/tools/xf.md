# xf - X Archive Search

Ultra-fast CLI for searching and querying your X (Twitter) data archive with sub-millisecond latency.

**Repository:** https://github.com/Dicklesworthstone/xf
**Language:** Rust
**Stars:** 65
**License:** MIT

## Overview

xf indexes your X (formerly Twitter) data export and provides blazingly fast full-text search across tweets, likes, DMs, and Grok conversations—all from the command line. It solves the problem that X's built-in archive viewer is slow and clunky.

## Key Features

- **Sub-Millisecond Search:** Tantivy-powered full-text search with BM25 ranking
- **Vector Similarity Search:** Hash-based vocabulary similarity by default; optional ML embeddings with MiniLM
- **Hybrid Search:** Combines keyword + vector similarity for comprehensive results
- **Search Everything:** Tweets, likes, DMs, and Grok conversations in one place
- **Rich Query Syntax:** Phrases, wildcards, boolean operators (AND, OR, NOT)
- **DM Context:** View full conversation threads with search matches highlighted
- **Multiple Output Formats:** JSON, CSV, compact, or colorized terminal output
- **Privacy-First:** All data stays local—nothing sent anywhere
- **Fast Indexing:** ~10,000 documents/second with parallel parsing

## Quick Install

```bash
curl -fsSL "https://raw.githubusercontent.com/Dicklesworthstone/xf/main/install.sh?$(date +%s)" | bash
```

Or via package managers:

```bash
# macOS/Linux (Homebrew)
brew install dicklesworthstone/tap/xf

# Windows (Scoop)
scoop bucket add dicklesworthstone https://github.com/Dicklesworthstone/scoop-bucket
scoop install dicklesworthstone/xf
```

## Quick Start

```bash
# 1. Get your X archive from X settings (takes 24 hours to prepare)
# Download the zip file (~500MB typical)

# 2. Index your archive (default: hash-based embeddings)
xf index ~/x-archive

# Optional: true semantic embeddings (downloads ~80MB on first use)
xf index ~/x-archive --semantic

# 3. Search
xf search "machine learning"                          # Hybrid search (default)
xf search "feeling overwhelmed at work" --mode semantic  # Vector similarity
xf search "rust async" --mode lexical                 # Keyword-only (BM25)
xf search "meeting tomorrow" --types dm --context     # DMs only
xf search "rust async" --format json --limit 50      # Export as JSON
```

## Use Cases for AI Agents

xf is particularly powerful for coding agents:

- **Context Building:** Agents can search your entire posting history to understand your preferences, tools, and workflows
- **Decision Support:** "What would our leader do?" — agents can consult your tweets and DMs as a knowledge base
- **Pattern Recognition:** Identify recurring solutions, tools, and approaches you've shared publicly
- **Project Context:** Understand architectural decisions and historical project discussions

## Search Modes

- `--mode hybrid` (default): BM25 + vector similarity
- `--mode lexical`: Keyword-only (BM25), best for exact terms
- `--mode semantic`: Vector similarity (hash by default, ML if indexed with --semantic)

## Agent Quickstart (JSON)

For agent use, always use `--format json`:

```bash
# Index once
xf index ~/x-archive

# Search with machine-readable output
xf search "machine learning" --format json --limit 20

# Get archive stats
xf stats --format json
```

## Why Use xf

- **Personal Knowledge Base:** Transform your X posting history into a searchable knowledge base
- **Institutional Memory:** For agents and teams, xf unlocks your historical context
- **Local Privacy:** All processing happens on your machine
- **Performance:** Sub-millisecond queries on massive archives
