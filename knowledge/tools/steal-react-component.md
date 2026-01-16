# Steal React Component - Claude Code Skill Suite

**Repository:** https://github.com/dennisonbertram/steal-react-component
**Stars:** 50
**Purpose:** Claude Code skill to extract React components from any production website

## Overview

A Claude Code skill suite for extracting and reconstructing React components and entire websites using browser automation and React Fiber internals. Enables 1:1 component cloning without needing source code access.

## Features

### Component Extraction (`steal-react-component`)
Extract individual React components from any production website by accessing React Fiber internals.

### Design System Extraction (`css-extractor`)
Extract complete design systems including CSS variables, typography, colors, and spacing.

### Full Site Cloning (`copy-site`)
Clone entire websites by combining component extraction, style extraction, and automatic project scaffolding.

### Visual Navigator
Interactive component browsing UI to select and preview components before extraction.

## Quick Start

```bash
# Extract a single component
/steal-react-component https://example.com

# Clone an entire site
/copy-site https://example.com
```

## Installation

### Two-File Architecture (Context Isolation)

| Skill | Dispatcher | Agent | Purpose |
|-------|------------|-------|---------|
| steal-react-component | SKILL.md (~300 tokens) | AGENT.md (~4k tokens) | Extract individual components |
| copy-site | COPY-SITE.md (~400 tokens) | COPY-SITE-AGENT.md (~6k tokens) | Clone entire websites |

The subagent architecture keeps the main agent's context clean, preventing token accumulation.

### Step 1: Install the Agents

Copy agent files to your Claude Code agents directory:

```bash
# User-level (available in all projects)
cp AGENT.md ~/.claude/agents/steal-react-component.md
cp COPY-SITE-AGENT.md ~/.claude/agents/copy-site.md

# Or project-level
cp AGENT.md .claude/agents/steal-react-component.md
cp COPY-SITE-AGENT.md .claude/agents/copy-site.md
```

### Step 2: Install the Skills

```bash
# User-level
mkdir -p ~/.claude/skills/steal-react-component
cp SKILL.md CSS-EXTRACTOR.md COPY-SITE.md ~/.claude/skills/steal-react-component/

# Or project-level
mkdir -p .claude/skills/steal-react-component
cp SKILL.md CSS-EXTRACTOR.md COPY-SITE.md .claude/skills/steal-react-component/
```

### Optional: Install as Commands

```bash
mkdir -p ~/.claude/commands
cp COPY-SITE.md ~/.claude/commands/copy-site.md
```

## Core Components

### SKILL.md + AGENT.md - ReactStealer
Core component extraction tool (split for token efficiency):
- Access React Fiber internals via `__reactFiber$*` keys
- Extract component props, hooks, HTML, and minified source
- Visual Navigator UI for interactive component browsing
- LLM-formatted output for clean code reconstruction

```javascript
// Inject ReactStealer, then:
ReactStealer.summary()           // List all components
ReactStealer.getForLLM('Button') // Get reconstruction prompt
```

### CSS-EXTRACTOR.md - StyleStealer
Design system extraction:
- CSS custom properties (design tokens)
- Typography system (fonts, sizes, weights)
- Color palette with semantic naming
- Direct Tailwind config generation

```javascript
// Inject StyleStealer, then:
StyleStealer.extractAll()       // Get full design system
StyleStealer.toTailwindConfig() // Generate Tailwind config
StyleStealer.toCSSVariables()   // Export as CSS file
```

### COPY-SITE.md + COPY-SITE-AGENT.md - Full Site Cloning
End-to-end site cloning workflow:
1. Screenshot and document the site
2. Extract design system with StyleStealer
3. Extract components with ReactStealer
4. De-minify with parallel subagents
5. Scaffold Next.js project
6. Verify the clone matches original

## How It Works

### The Technique

1. **Two Trees** - React maintains a Fiber tree parallel to the DOM
2. **Fiber Access** - React attaches Fiber nodes via `__reactFiber$*` keys
3. **Data Extraction** - Extract component type, props, hooks, rendered HTML
4. **Style Extraction** - Pull CSS variables, computed styles, typography
5. **Example Collection** - Gather multiple prop→HTML mappings
6. **LLM Reconstruction** - Feed examples + minified source to LLM
7. **Project Scaffolding** - Generate complete Next.js project
8. **Verification** - Compare rendered output until it matches

## Requirements

- Claude Code CLI (started with `claude --chrome`)
- Chrome browser with [Claude-in-Chrome](https://github.com/anthropics/claude-in-chrome) extension
- Target website (React apps work best, any site works for style extraction)

## Use Cases

- Extracting components from competitor websites
- Building design systems from existing applications
- Rapid prototyping based on production UI patterns
- Learning from well-designed component architecture
- Full website cloning and reimplementation
