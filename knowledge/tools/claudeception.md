# Claudeception

## Overview
Claudeception is a Claude Code skill that enables autonomous skill extraction and continuous learning. It allows Claude Code to discover solutions, save them as reusable skills, and automatically load those skills in future sessions to avoid re-learning the same problems.

## Problem It Solves
Typical AI agent workflows start from zero each session. Time spent debugging an issue is lost when the session ends. Next time you hit the same problem, the agent has no memory of the solution.

Claudeception solves this by creating persistent skill libraries that carry knowledge across sessions.

## Key Features
- **Automatic skill extraction**: Detects when Claude Code discovers non-obvious solutions
- **Knowledge persistence**: Saves learned patterns as reusable skills
- **Semantic matching**: Automatically loads relevant skills based on context
- **Activation hooks**: Optional system hook to evaluate every session for extractable knowledge
- **Quality gates**: Only extracts knowledge that's genuinely useful and verified

## What Gets Extracted
Skills are created only when:
- Debugging discovered a non-obvious solution
- A workaround was found through investigation
- Root cause wasn't immediately apparent
- Project-specific patterns were learned
- Task solution required meaningful discovery (not just documentation lookup)

## Installation
```bash
# User-level (recommended)
git clone https://github.com/blader/Claudeception.git ~/.claude/skills/claudeception

# Project-level
git clone https://github.com/blader/Claudeception.git .claude/skills/claudeception
```

## Activation Hook Setup
1. Create hooks directory:
```bash
mkdir -p ~/.claude/hooks
cp ~/.claude/skills/claudeception/scripts/claudeception-activator.sh ~/.claude/hooks/
chmod +x ~/.claude/hooks/claudeception-activator.sh
```

2. Add to `~/.claude/settings.json`:
```json
{
  "hooks": {
    "UserPromptSubmit": [
      {
        "hooks": [
          {
            "type": "command",
            "command": "~/.claude/hooks/claudeception-activator.sh"
          }
        ]
      }
    ]
  }
}
```

## Usage

### Automatic Mode
Activates when Claude Code:
- Completes debugging and discovers non-obvious solution
- Finds workaround through investigation
- Resolves error where root cause wasn't apparent
- Learns project-specific patterns
- Completes task with meaningful discovery

### Explicit Mode
```
/claudeception
```
Or request directly:
```
Save what we just learned as a skill
```

## Skill Format
Skills are markdown files with YAML frontmatter:
```yaml
---
name: prisma-connection-pool-exhaustion
description: |-
  Fix for PrismaClientKnownRequestError: Too many database connections
  in serverless environments. Use when connection count errors appear.
author: Claude Code
version: 1.0.0
date: 2024-01-15
---

# Skill Name

## Problem
[Description of issue]

## Context / Trigger Conditions
[Exact error messages and scenarios]

## Solution
[Step-by-step fix]

## Verification
[How to confirm it worked]
```

## Skill Description Best Practices
- Specific and trigger-focused: "Fix for PrismaClientKnownRequestError in serverless" works better than "Helps with database problems"
- Include error messages and version numbers
- Mention specific frameworks and environments
- Optimize for semantic matching in future sessions

## How It Works
Claude Code has a native skills system:
1. At startup, loads skill names and descriptions (~100 tokens each)
2. During work, matches current context against descriptions
3. Pulls in relevant skills automatically
4. Skill descriptions are optimized for future retrieval

## Research Foundation
Based on academic work on skill libraries for AI agents:
- **Voyager** (Wang et al., 2023): Game-playing agents benefit from skill libraries
- **CASCADE** (2024): Introduces meta-skills (skills for acquiring skills)
- **SEAgent** (2025): Agents learn new environments through trial and error
- **Reflexion** (Shinn et al., 2023): Self-reflection improves performance

## Repository
https://github.com/blader/Claudeception

## Language
Shell

## Stars
1,080+

## Creator
[Siqi Chen](https://x.com/blader) (@blader)

## License
MIT (inferred from reference in repository documentation)

## Key Insight
Agents that persist what they learn perform better than agents starting fresh each session.
