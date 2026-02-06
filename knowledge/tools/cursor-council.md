# Cursor /council Command

**URL:** https://shaoruu.io/cursor/council

The `/council` command in Cursor spawns multiple agents to deeply explore a codebase area before taking action. It's designed for comprehensive code analysis and understanding before making changes.

## How It Works
1. Analyze the given area of interest
2. Gather general information (keywords, architecture overview)
3. Spawn n=10 task agents (configurable) to dig deeper
4. Some agents work out-of-the-box for variance
5. Use gathered information to accomplish the user's goal

## Use Cases
- Understanding a complex codebase area
- Planning changes in unfamiliar code
- Comprehensive code analysis before refactoring
- Reducing risk of unintended side effects

## Part of Cursor Resources
Created by @shaoruu (Ian Huang) as part of Cursor's command library. Includes other commands like:
- /general-push
- /fix-bugbot-comments
- /iterate-browser
- /fix-ci
- /you-might-not-need-an-effect

## Reference
- Mentioned by: @rudrank (Rudrank Riyam)
- Status: Active command in Cursor
