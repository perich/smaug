# Find Skills - Vercel Labs

## Overview
find-skills is a skill for discovering and installing skills from the open agent skills ecosystem. It helps agents understand when and how to search for specialized capabilities.

## Purpose
Use this skill when users ask:
- "How do I do X" where X might have an existing skill
- "Find a skill for X" or "is there a skill for X"
- "Can you do X" for specialized capabilities
- Want to extend agent capabilities
- Search for tools, templates, or workflows
- Mention needing help with specific domains (design, testing, deployment, etc.)

## The Skills CLI
`npx skills` is the package manager for the open agent skills ecosystem. Skills are modular packages that extend agent capabilities.

### Key Commands
- `npx skills find [query]` - Search for skills interactively or by keyword
- `npx skills add <package>` - Install a skill from GitHub or other sources
- `npx skills check` - Check for skill updates
- `npx skills update` - Update all installed skills

## How to Use

### Step 1: Understand What They Need
- Identify the domain (e.g., React, testing, design, deployment)
- Identify the specific task (e.g., writing tests, creating animations, reviewing PRs)
- Determine if this is common enough that a skill likely exists

### Step 2: Search for Skills
Run find command with relevant queries:
```bash
npx skills find [query]
```

Examples:
- User asks "how do I make my React app faster?" → `npx skills find react performance`
- User wants testing help → `npx skills find testing`

## Installation
You can install as a Claude Code plugin:
```bash
npx skills add https://github.com/vercel-labs/skills --skill find-skills
```

## Key Insight
Skills enable agents to loop independently with specific goals. Rather than telling an agent what to do, give it success criteria and access to the right skills.

## Browse Skills
Find more skills at: https://skills.sh/

## Source
https://skills.sh/vercel-labs/skills/find-skills
