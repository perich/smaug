# DocSetQuery

Local-first Apple documentation extraction tool for agent workflows.

**Repository:** [PaulSolt/DocSetQuery](https://github.com/PaulSolt/DocSetQuery)
**Stars:** 75
**Language:** Python

## What it does

Extracts and cleans up Apple DocC documentation from local Dash docsets into predictable, citeable Markdown format. Built specifically for agent workflows that need deterministic documentation without web scraping.

## Key features

- Export DocC content from Apple docset to Markdown
- Sanitize exports with cleaned front matter and trimmed table of contents
- Build JSON index for fast local search by heading/section
- Instant lookup without re-reading docsets for every query
- Sync canonical docs cache into repository cache

## Why use it

- Apple docs are large and dynamic; agents need stable, local references
- DocC exports are noisy; predictable front matter and cleaned TOC are essential
- Local search is instant, avoiding remote doc fetching during agent runs
- Deterministic output keeps agent prompts consistent

## Usage example

```bash
# Export a framework/topic tree to Markdown
python tools/docset_query.py export \
  --root /documentation/vision \
  --output docs/apple/vision.md

# Sanitize the export (trim TOC, rebuild front matter)
python tools/docset_sanitize.py --input docs/apple/vision.md --in-place --toc-depth 2

# Build or refresh the search index
python tools/docindex.py rebuild

# Search headings/key sections
python tools/docindex.py search "CVPixelBuffer"
```

## Agent workflow

1. Search locally first with `docindex.py search` against `docs/apple`
2. Fetch only what's missing with `docset_query.py fetch` or `export`
3. Sanitize output to keep front matter and TOC consistent
4. Rebuild index for fast agent search
5. Keep canonical cache via `sync_docs.sh`

## Configuration

- **Docset path:** `~/Library/Application Support/Dash/DocSets/Apple_API_Reference/`
- **Default language:** Swift
- **Cache location:** `~/.cache/apple-docs`
- **Export depth:** 7 (configurable)

## Use case

Perfect for AI agents that need grounded Apple API references with stable citations and fast local lookups.
