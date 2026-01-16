# Why We Built Our Own Background Agent

**Source:** https://builders.ramp.com/post/why-we-built-our-background-agent
**Authors:** Zach Bruggeman, Jason Quense, Rahul Sengottuvelu
**Date:** January 12, 2026

## Overview

Ramp built their own background coding agent called Inspect that has achieved remarkable adoption. The agent wrote 30% of merged frontend and backend PRs in their core repositories within the first week, without being mandatory.

## Key Technical Details

- **Architecture:** Runs fully in the cloud with fast startup times
- **Dependencies:** Powered by OpenCode, Modal, and Cloudflare
- **Performance:** No setup required; sessions start in seconds
- **Open Source:** The full blueprint is available for others to implement

## Core Insights

### 1. Agents as Control Systems
The most important insight is viewing agents as control systems where generating output is easy—feedback is everything. Inspect doesn't just propose diffs; it iterates until evidence (tests, telemetry, feature flags) confirms the change is correct.

### 2. Power of Cheap, Parallel Sessions
When agents run in sandboxed cloud environments rather than locally:
- Developers stop babysitting single solutions
- They can run more parallel iterations without resource rationing
- Multiple versions of the same prompt can be tested simultaneously
- Teams can swap models and try approaches without hesitation

### 3. Multi-Client and Multiplayer Architecture
Integration across existing tools matters more than standalone capability:
- Shows up where work already happens (PRs, Slack, web, VS Code)
- Sessions can be handed to teammates
- Becomes shared infrastructure rather than a novelty
- Adoption across job functions (not just engineers) demonstrates broad value

## Adoption Metrics

- ~30% of merged PRs authored by Inspect (without mandates)
- Contributors include people from essentially every job function
- Organic adoption pattern

## Why Open Source the Blueprint

By sharing their specification, Ramp enabled any coding agent to implement the Inspect architecture, democratizing the approach.
