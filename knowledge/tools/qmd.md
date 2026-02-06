# QMD - Query Markup Documents

**GitHub:** https://github.com/tobi/qmd
**Stars:** 6587
**Language:** TypeScript

## Overview
QMD is a hybrid search engine for markdown knowledge bases, combining BM25 full-text search, vector semantic search, and LLM re-ranking—all running locally via node-llama-cpp with GGUF models. Ideal for indexing personal notes, meeting transcripts, documentation, and knowledge bases.

## Key Features
- **Hybrid search pipeline:** Original query (×2 weight) + 2 query expansions through 3 parallel search paths (BM25, vector search, combined)
- **Local processing:** All search happens on-device using GGUF models
- **Multiple interfaces:** CLI, MCP server, and Claude Desktop integration
- **Collection management:** Organize docs into named collections with contextual metadata
- **Flexible retrieval:** Search by keywords or natural language, retrieve by path, docid, or glob patterns

## Quick Commands
```bash
qmd collection add ~/notes --name notes
qmd embed  # Generate embeddings
qmd search "topic"  # Keyword search
qmd vsearch "question"  # Semantic search
qmd query "topic"  # Hybrid search with reranking
qmd get "path/to/doc.md"  # Retrieve specific document
qmd search "API" --json -n 10  # Structured output for agents
```

## Integration
- **Claude Desktop:** Add to `claude_desktop_config.json`
- **Claude Code:** Install via marketplace or configure in `~/.claude/settings.json`
- **Tools exposed:** `qmd_search`, `qmd_vsearch`, `qmd_query`, `qmd_get`, `qmd_multi_get`, `qmd_status`

## Use Cases
- Personal knowledge base search across notes and documentation
- Meeting transcript indexing and retrieval
- Agent-friendly document retrieval with structured JSON output
- Local semantic search without external API dependencies
