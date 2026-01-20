# How to write a good spec for AI agents

**Author:** Addy Osmani
**Source:** https://addyosmani.com/blog/good-spec/
**Date:** January 13, 2026

## Overview

A comprehensive guide on writing effective specifications for AI coding agents. Rather than overwhelming agents with massive specs, focus on smart, focused specifications that guide clearly while respecting context window limits and the model's attention budget.

## Key Principles

### 1. Start with high-level vision and let the AI draft the details

Begin with a clear goal statement and core requirements, then have the agent expand into detailed plans. This leverages AI's strength in elaboration while maintaining directional control. The spec becomes a living artifact that both developer and agent refine together.

**Practical approach:**
- Start with a product brief rather than full specification
- Ask the AI to draft a detailed specification covering objectives, features, constraints, and step-by-step plan
- Keep initial prompts high-level (e.g., "Build a web app where users can track tasks")
- Review and refine the AI's spec before proceeding

### 2. Spec-driven development

GitHub's approach: "Specs become the shared source of truth... living, executable artifacts that evolve with the project." Before writing code, have the AI review and refine the spec, clarifying ambiguities.

### 3. Plan Mode for planning-first

Tools like Claude Code offer Plan Mode that restricts agents to read-only operations. Use this to:
- Analyze existing codebase
- Create detailed plans
- Clarify ambiguities before code execution
- Get clear understanding before implementation

## Key Takeaway

**Aim for a clear spec covering just enough nuance (structure, style, testing, boundaries) to guide the AI without overwhelming it. Break large tasks into smaller ones rather than keeping everything in one large prompt. Plan first in read-only mode, then execute and iterate continuously.**
