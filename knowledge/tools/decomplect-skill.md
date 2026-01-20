# Decomplect Claude Code Skill

**Author/Source:** Shane Evans (shanev)
**Repository:** https://github.com/shanev/skills
**Collection:** Shane's Claude Code Skills

## Overview

A Claude Code skill for architectural code analysis and design quality assessment. Part of a collection of skills designed to enhance development workflows through AI-guided architectural improvements.

## Purpose

Decomplect performs architectural analysis focused on design quality, helping identify and fix code that violates clean architecture principles.

## Key Principles

### Simplicity
- Values over state
- Decomplected concerns
- Clear separation of responsibility

### FCIS (Functional Core, Imperative Shell)
- Pure business logic separate from effects
- Easy to test and reason about
- Clear data flow

### Coupling
- High cohesion (related functionality together)
- Low coupling (minimal interdependencies)
- Modular design

## Usage

```
/decomplect
```

Provides architectural analysis and recommendations for improving code design quality.

## Installation

Available through Claude Code plugin marketplace:
```bash
/plugin marketplace add shanev/skills
/plugin install decomplect@shanev-skills
```

## Related Skills

Also available from the same author:
- **Unslopify** - Tactical code cleanup for immediate quality issues
  - Type strictness (no `any`, domain types)
  - Single responsibility (no god classes)
  - Fail-fast patterns (no silent fallbacks)
- **Tmux-task-runner** - Task execution and management

## Context

Developed in response to broader discussions about code quality for AI agents, particularly around making code more testable and maintainable through proper architectural patterns.
