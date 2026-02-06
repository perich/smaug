# Andrej Karpathy Guidelines for Coding Agents

## Overview
Guidelines for improving Claude Code behavior, derived from Andrej Karpathy's observations on LLM coding pitfalls. A set of principles designed to reduce common LLM mistakes in code generation.

## The Problems Addressed

From Andrej Karpathy's observations:
- Models make wrong assumptions and run with them without checking
- Don't manage confusion or seek clarifications
- Don't surface inconsistencies or present tradeoffs
- Overcomplicate code and APIs, bloat abstractions
- Sometimes remove or change comments/code they don't understand as side effects

## Four Core Principles

### 1. Think Before Coding
**Don't assume. Don't hide confusion. Surface tradeoffs.**

- State assumptions explicitly — ask rather than guess when uncertain
- Present multiple interpretations — don't pick silently when ambiguity exists
- Push back when warranted — suggest simpler approaches when they exist
- Stop when confused — name what's unclear and ask for clarification

### 2. Simplicity First
**Minimum code that solves the problem. Nothing speculative.**

- No features beyond what was asked
- No abstractions for single-use code
- No "flexibility" or "configurability" that wasn't requested
- No error handling for impossible scenarios
- If 200 lines could be 50, rewrite it

**Test**: Would a senior engineer say this is overcomplicated? If yes, simplify.

### 3. Surgical Changes
**Touch only what you must. Clean up only your own mess.**

When editing existing code:
- Don't "improve" adjacent code, comments, or formatting
- Don't refactor things that aren't broken
- Match existing style, even if you'd do it differently
- If you notice unrelated dead code, mention it — don't delete it

When your changes create orphans:
- Remove imports/variables/functions that YOUR changes made unused
- Don't remove pre-existing dead code unless asked

**Test**: Every changed line should trace directly to the user's request.

### 4. Goal-Driven Execution
**Define success criteria. Loop until verified.**

Transform imperative tasks into verifiable goals with tests:

| Instead of... | Transform to... |
|---------------|-----------------|
| "Add validation" | "Write tests for invalid inputs, then make them pass" |
| "Fix the bug" | "Write a test that reproduces it, then make it pass" |
| "Refactor X" | "Ensure tests pass before and after" |

For multi-step tasks, state a brief plan with verification points.

## How to Know It's Working

- Fewer unnecessary changes in diffs — only requested changes appear
- Fewer rewrites due to overcomplication — code is simple the first time
- Clarifying questions come before implementation — not after mistakes
- Clean, minimal PRs — no drive-by refactoring or "improvements"

## Installation

**Option A: Claude Code Plugin (recommended)**
```bash
npx skills add https://github.com/forrestchang/andrej-karpathy-skills
```

**Option B: CLAUDE.md (per-project)**
```bash
curl -o CLAUDE.md https://raw.githubusercontent.com/forrestchang/andrej-karpathy-skills/main/CLAUDE.md
```

Or append to existing CLAUDE.md:
```bash
echo "" >> CLAUDE.md
curl https://raw.githubusercontent.com/forrestchang/andrej-karpathy-skills/main/CLAUDE.md >> CLAUDE.md
```

## Key Insight
From Andrej: "LLMs are exceptionally good at looping until they meet specific goals... Don't tell it what to do, give it success criteria and watch it go."

The "Goal-Driven Execution" principle captures this: transform imperative instructions into declarative goals with verification loops.

## Customization
These guidelines are designed to be merged with project-specific instructions. Add them to your existing CLAUDE.md or create a new one.

## Source
https://github.com/forrestchang/andrej-karpathy-skills

## Related
- Author: Forrest Chang
- Based on: Andrej Karpathy's observations on LLM coding pitfalls
