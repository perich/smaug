---
title: "The Ralph Wiggum Approach to Long-Running AI Coding Agents"
type: article
date_added: 2026-01-05
source: "https://x.com/mattpocockuk/status/2007924876548637089"
tags: [ai-agents, coding, automation, agentic-development, long-running-tasks, bash-scripting]
via: "Twitter bookmark from @mattpocockuk"
---

## Overview

The "Ralph Wiggum approach" is a method for running long-duration AI coding agents (hours or days) that autonomously ship code while you sleep or work on other tasks. Developed and documented by Matt Pocock, it combines bash scripting, Product Requirements Documents (PRDs), progress tracking, and CI/CD integration to enable truly autonomous feature development.

The name references Ralph Wiggum's chaotic energy—the agent runs repeatedly with a clean slate, again and again, until a stop condition is met, generating progress through sheer iteration.

## Core Principles

### 1. Iterative Clean-Slate Execution

- Set up a bash for loop that runs a defined number of times (e.g., 10 iterations)
- Choose a finite number to prevent infinite loops
- Each iteration gives the coding agent a fresh context window
- The agent works on a single feature until completion

### 2. Stop Conditions

Three approaches to tell the LLM when to stop:

**Raw Prompting**: Pass clear stop conditions directly
```
"The job is complete when X conditions are met"
```

**TODO List**: Give the agent an explicit task list to complete

**PRD-Based** (Recommended): Use a JSON file of user stories with `passes: false` status

### 3. Progress Reporting

**Critical for long-running agents:**
- Agent MUST commit its work after each feature
- Agent MUST append progress to `progress.txt` file
- Use verb "append" to preserve history (not overwrite)
- Git history shows exactly what each iteration accomplished
- Future agent iterations can understand prior work through commits

### 4. Keep CI Green

**Every commit must pass:**
- All tests
- Type checking
- Linting (if applicable)

Failure to maintain CI health causes problems:
- Future agents inherit buggy code
- Agents waste time bisecting to find bugs
- Code quality degrades through iterations

This means building really healthy feedback loops is CRITICAL.

## The PRD Approach (Recommended)

### The Problem

Two immediate issues with naive Ralph:

1. **Scope Creep**: The agent picks tasks that are too large, too ambitious. It runs out of context window and fails.
2. **Stopping**: The agent doesn't know when to stop—no natural completion signal.

### The Solution: JSON-Based PRD

Create a JSON file of user stories:

```json
{
  "stories": [
    {
      "id": "auth-login",
      "title": "User login functionality",
      "description": "...",
      "passes": false
    },
    {
      "id": "profile-update",
      "title": "User can update profile",
      "description": "...",
      "passes": false
    }
  ]
}
```

### Execution Pattern

1. Agent picks the highest-priority unfinished feature
2. Agent works ONLY on that single feature
3. After completing that feature, agent updates the `passes: true` status in the PRD
4. Next iteration, agent picks next feature
5. Continue until all stories pass: true

### Benefits

- **Scope Control**: Each iteration focuses on one feature, using only small part of context window
- **No Context Rot**: Agent isn't swamped by gigabytes of prior context
- **Clear Progress**: PRD file is human-readable progress tracker
- **Prioritization**: Ability to weight features by importance
- **Flexibility**: Can add new stories mid-run; agent adapts

## Implementation Summary

Four essential components:

### 1. Bash Script
```bash
for i in {1..10}; do
  # Call coding agent with PRD
  # Check for <promise>COMPLETE</promise>
  # Exit early if found
done
```

### 2. JSON-Based PRD
Formal specification of work: user stories with completion tracking

### 3. Progress.txt File
Append-only log of all work completed across iterations

### 4. Healthy Feedback Loops
- Tests must pass
- Types must pass
- Clean commits with meaningful messages
- Future agents can understand the work

## Why "Ralph Wiggum"?

Ralph Wiggum (from The Simpsons) represents chaotic energy and repetition—he's famous for doing the same thing over and over without self-awareness. The approach embraces this: throw an agent at the problem repeatedly until it's solved. The structure (PRD, progress.txt, CI) provides the guardrails that prevent chaos.

## Advantages Over Manual Development

- **24/7 Development**: Code ships while you sleep
- **Context Efficiency**: PRD-based scoping prevents context waste
- **Audit Trail**: Every commit and progress entry is tracked
- **Reproducibility**: Future runs can understand exactly what happened
- **Scalability**: Once configured, can run repeatedly without human intervention

## Challenges and Mitigations

| Challenge | Mitigation |
|-----------|-----------|
| Agent gets stuck | Finite loop count prevents infinite loops; human intervention if needed |
| Bad code spreads | Keep CI green requirement prevents inheritance of bugs |
| Lost context | progress.txt + git history + PRD provides complete record |
| Scope explosion | PRD-based approach forces task-by-task focus |
| Token waste | Small context window per iteration due to scoped features |

## When to Use Ralph Wiggum

Ideal for:
- Feature-focused development with clear acceptance criteria
- Projects with good test coverage
- Autonomous task completion overnight
- Continuous deployment pipelines
- Well-scoped feature work (not architectural refactoring)

Less ideal for:
- Architectural decisions requiring human judgment
- Highly ambiguous or exploratory work
- Projects with poor test coverage
- Code that requires deep domain knowledge

## Related Concepts

- **Agent Flywheel Setup (ACFS)**: Multi-agent orchestration tools (ntm, cass, bv) that complement Ralph
- **Claude Code/Codex**: The underlying agents that execute the work
- **Clawdbot**: Personal assistant that can run Ralph workflows through chat interfaces

## Links

- [Original Tweet Thread](https://x.com/mattpocockuk/status/2007924876548637089)
- [Agent Flywheel Setup](https://github.com/Dicklesworthstone/agentic_coding_flywheel_setup)
- [Matt Pocock Twitter](https://x.com/mattpocockuk)
