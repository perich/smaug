---
title: "Agent Flywheel"
type: tool
date_added: 2026-01-05
source: "https://agent-flywheel.com/"
tags: [ai-development, coding-agents, claude-code, vps-setup, workflow-automation, team-coordination]
via: "Twitter bookmark from @doodlestein"
---

Agent Flywheel is a complete, free, open-source system for transforming a cloud server into a fully-configured agentic coding environment. It provides comprehensive setup instructions, tool integrations, and workflows designed to enable multiple AI coding agents (Claude Code, OpenAI Codex, Google Gemini) to collaborate effectively on complex software projects.

Created by Jeffrey Emanuel, the system automates the infrastructure setup and provides proven workflows for planning, task management, implementation, and review cycles that have demonstrated the ability to produce production-grade software at team-level velocity.

## Key Components

- **Server Setup** - Complete VPS configuration for agentic coding environments
- **Multi-Agent Coordination** - Integration with MCP Agent Mail for inter-agent communication
- **Tool Integration** - 30+ modern developer tools pre-configured
- **Workflow Automation** - TMux integration and NTM abstractions for parallel agent sessions
- **Task Management** - "Beads" system (epics/tasks/subtasks) optimized for AI agent workflows

## The Complete Workflow

1. **Planning Phase**
   - Write markdown project plan
   - Use ChatGPT 5.2 Pro with extended reasoning to critique and improve the plan
   - Iterate 4-5 rounds until plan reaches steady-state

2. **Task Decomposition**
   - Use Claude Code with Opus 4.5 to convert plan into "beads" (granular tasks with dependencies)
   - Include detailed comments and reasoning for future understanding
   - Verify task structure makes sense

3. **Implementation Phase**
   - Launch multiple agent sessions (Claude Code, Codex, Gemini-CLI) in parallel
   - Agents coordinate via MCP Agent Mail
   - Agents track progress via beads and mark completion
   - Implement verification/testing systems as work progresses

4. **Review Cycles**
   - Agents perform fresh-eyes code review after implementation
   - Check for bugs, inefficiencies, security issues
   - Integrate feedback into next bead iterations
   - Continue until reviews come clean

5. **Refinement**
   - Once implementation complete, run additional rounds:
     - Code quality and best practices audit
     - UI/UX polish and optimization
     - Random deep dives into code for edge cases
     - Cross-agent code review for peer feedback
     - Test coverage improvements

## Key Innovations

- **Beads System** - Task representation optimized for AI agents rather than humans
- **Agent Mail** - Lightweight inter-agent communication preventing "communication purgatory"
- **Tool Verification** - Built-in methods for agents to verify their own outputs
- **Iterative Improvement** - Structured rounds of review and refinement
- **Parallelization** - Multiple agents working simultaneously with clear coordination

## Technical Details

- **Setup Cost** - Free (code) + ~$500/month (Claude Max + GPT Pro + VPS)
- **VPS Requirement** - Any cloud provider; typically $50/month
- **Language Support** - JavaScript/TypeScript primary, extensible to others
- **Architecture** - Decentralized agent coordination, no central controller
- **Version Control** - Git-based with detailed, atomic commits

## Results and Impact

According to the creator, following this system has enabled:
- Production-grade software delivery in 1-2 days (what would normally take teams weeks)
- GitHub profiles appearing as if built by 100+ developers
- Consistent, high-quality outputs across multiple projects
- Proven patterns for handling edge cases and refinement

## Use Cases

- Building complete applications from scratch
- Rapid prototyping with high code quality
- Multi-feature development with parallel agents
- Projects requiring extensive testing and refinement
- Complex systems requiring cross-cutting concerns

## Significance

Agent Flywheel demonstrates that the frontier models are already capable of generating production-quality software at scale. The key is not better models but better workflows, tooling, and coordination patterns. It represents a practical blueprint for organizations wanting to leverage AI for software development at team-level velocity.

## Links

- [Website](https://agent-flywheel.com/)
- [GitHub](https://github.com/Dicklesworthstone/agentic_coding_flywheel_setup)
- [Original Tweet](https://x.com/doodlestein/status/2007588870662107197)

