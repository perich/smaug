# Claude Skills - Swift Server Linting and Best Practices

**Repository:** https://github.com/Joannis/claude-skills
**Author:** Joannis
**Language:** Swift
**Stars:** 48

## Overview

Claude Skills is a repository containing Claude skills for guidance on Swift (Server) development paired with a linting tool that enforces best practices through automated rule checking. It demonstrates an effective feedback loop for improving LLM-generated code quality.

## Core Concept

The repository implements a technique for ensuring consistent code quality from LLM-generated code:

1. **Define code standards** - Establish what "good" code looks like for your project
2. **Add as Claude Skills** - Encode standards as expert guidance for the LLM
3. **Convert to linter rules** - Automatically enforce standards through automated linting

This creates a feedback loop where Claude generates code that adheres to defined standards, and linter rules catch violations independently of the LLM's context window.

## Components

### 1. Skills

Knowledge bases that provide expert guidance on Swift server development topics. These skills inform Claude's code generation to follow best practices and project conventions.

### 2. swift-server-lint

A linting tool that enforces best practices from the skills through automated code analysis. This ensures consistency even when skills aren't in the LLM's context window.

## Key Principle

The approach addresses a fundamental challenge with LLM-assisted coding: while LLMs can make mistakes, the solution isn't complaint—it's systematic improvement through:

- **Articulation**: Document what should be improved and why
- **Codification**: Add the rationale to Claude skills
- **Automation**: Encode rules as linter checks

This proves more effective than repeatedly asking the LLM to try again, as it creates persistent constraints the LLM learns from during the conversation and that persist across future generations.

## Use Cases

- Swift server application development
- Swift package development
- Server-side Swift best practices
- Linter rule development for Swift projects
- LLM-assisted Swift coding workflows

## Integration with Claude

The skills format works with Claude's context window to provide guidance during code generation sessions, while the linter ensures enforcement across multiple generations and developers.
