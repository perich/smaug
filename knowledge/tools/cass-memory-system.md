# CASS Memory System - Procedural Memory for AI Coding Agents

Transforms scattered agent sessions into persistent, cross-agent memory—so every agent learns from every other agent's experience.

**Repository:** https://github.com/Dicklesworthstone/cass_memory_system
**Language:** TypeScript
**Runtime:** Bun
**Status:** Alpha
**Stars:** 209
**License:** MIT

## Overview

CASS implements a three-layer cognitive architecture that transforms raw session logs into actionable, confidence-tracked rules:

| Layer | Role | Implementation |
|-------|------|-----------------|
| **Episodic Memory** | Raw ground truth from all agents | `cass` search engine |
| **Working Memory** | Structured session summaries | Diary entries |
| **Procedural Memory** | Distilled rules with tracking | Playbook bullets |

This mirrors how human expertise develops: raw experiences (episodic) are consolidated into structured memories (working), which eventually become automatic knowledge (procedural).

## The Problem It Solves

AI coding agents accumulate valuable knowledge through sessions but lose it when the session ends:

- Knowledge is **trapped in sessions** — Each session ends, context is lost forever
- Knowledge is **agent-specific** — Claude Code doesn't know what Cursor learned yesterday
- Knowledge is **unstructured** — Raw conversation logs aren't actionable as guidance
- Knowledge is **subject to collapse** — Naive summarization loses critical nuances

Example: You've solved authentication bugs three times this month across different agents, but each time you started from scratch.

## Key Features

- **Cross-Agent Learning:** Agents share knowledge discovered by other agents
- **Procedural Rules:** Distilled patterns with confidence tracking
- **Smart Onboarding:** Convert raw sessions into actionable playbooks
- **Trauma Guard:** Safety system to prevent harmful or low-confidence rules
- **Privacy-First:** All data stays local
- **Flexible Integration:** Works with Claude Code, Cursor, Aider, and other tools

## Quick Install

**One-liner (Linux/macOS):**

```bash
curl -fsSL "https://raw.githubusercontent.com/Dicklesworthstone/cass_memory_system/main/install.sh?$(date +%s)" \
  | bash -s -- --easy-mode --verify
```

**Or via package managers:**

```bash
# macOS/Linux (Homebrew)
brew install dicklesworthstone/tap/cm

# Windows (Scoop)
scoop bucket add dicklesworthstone https://github.com/Dicklesworthstone/scoop-bucket
scoop install dicklesworthstone/cm
```

## Agent Quickstart (JSON)

Always use `--json` in agent contexts. stdout = data, stderr = diagnostics, exit 0 = success.

```bash
# 1) Get task-specific memory before you start
cm context "implement auth rate limiting" --json

# 2) See the minimum viable workflow
cm quickstart --json

# 3) Build the playbook (memory onboarding)
cm onboard status --json
cm onboard sample --fill-gaps --json
cm onboard read /path/to/session.jsonl --template --json
cm onboard mark-done /path/to/session.jsonl
```

## Core Workflow

### Building Memory

1. **Capture Sessions:** All agent sessions are logged automatically
2. **Extract Summaries:** Structured episodic memory from raw logs
3. **Create Playbooks:** Distill learned rules with confidence tracking
4. **Share Knowledge:** Other agents access rules and patterns

### Using Memory

1. **Context Queries:** `cm context "your task"` returns relevant rules
2. **Playbook Assembly:** Agents use rules as building blocks
3. **Feedback Loop:** Outcomes inform confidence scores

## Data Models

CASS tracks:

- **Sessions:** Raw conversations with timestamps and outcomes
- **Diary Entries:** Structured summaries (accomplishments, decisions, challenges)
- **Playbook Bullets:** Distilled rules with source tracking and confidence
- **Outcomes:** Success/failure metrics to tune rules

## Who Benefits

- **AI Agents:** Get relevant rules and historical context before starting any task
- **Developers:** Build institutional memory that persists across tools and sessions
- **Teams:** Share patterns discovered by any team member's AI assistant
- **Power Users:** Create sophisticated workflows that leverage cross-agent learning

## Use Cases

- **Bug Fixing Patterns:** "Last time I encountered this error, here's what worked"
- **Architecture Decisions:** "Here's how we structure this type of service"
- **Workflow Optimization:** "When facing deadline pressure, use these techniques"
- **Tool Integration:** "Here's the exact setup for getting X tool working"
- **Code Style:** "Our team prefers these patterns for this language"

## Integration

CASS integrates with:

- Claude Code
- Cursor
- Aider
- Other AI coding agents via JSONL session format

## Key Characteristics

- **Procedural Learning:** Transforms episodic experiences into actionable procedures
- **Confidence Tracking:** Rules include success metrics and applicability conditions
- **Safety First:** Trauma Guard prevents low-confidence or harmful rules from being used
- **Cross-Domain:** Applicable to any coding task, not just language-specific
- **Persistent:** Memory survives across sessions, agents, and tools
