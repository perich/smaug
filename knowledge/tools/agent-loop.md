# Agent Loop

**Repo:** bentossell/agent-loop
**Language:** Shell
**Stars:** 49
**URL:** https://github.com/bentossell/agent-loop

General-purpose autonomous task execution system inspired by Matt Pocock's Ralph loop. Create GitHub Issues, run the loop, get PRs.

## How It Works

1. **You** create GitHub Issues describing tasks
2. **Loop** picks up issues and executes them
3. **PRs** are created, issues are closed

The issue body IS the specification. It can be anything:
- Bug fixes
- Feature requests
- Full PRDs
- Content to create
- Refactoring tasks

## Quick Start

### Option 1: GitHub Actions (Recommended)

Just create an issue - the workflow triggers automatically:

```bash
gh issue create --title "Add dark mode" --body "Add dark mode toggle to settings page..."
```

**Setup:**
1. Fork/clone this repo
2. Add `FACTORY_API_KEY` to repo secrets (Settings → Secrets → Actions)
3. Create issues - droid runs automatically

### Option 2: Local

```bash
# Install droid
curl -fsSL https://get.factory.ai | sh

# Set API key
export FACTORY_API_KEY="your-key"

# Create an issue and run
gh issue create --title "Add dark mode" --body "Add dark mode toggle to settings page..."
./loop.sh 10
```

## Customization

Edit `prompt.md` to customize the workflow:

### Feedback Loops
Add your project's test/build commands in Step 5:
```bash
npm run test
npm run build
```

### Priority Rules
Edit Step 2 to change how issues are prioritized by labels

### Commit Style
Edit Step 7 to match your commit conventions

## Usage Patterns

- **Single Task:** `./loop.sh 1`
- **Run Until Done:** `./loop.sh 50`
- **Background (AFK Mode):** `nohup ./loop.sh 100 > loop.log 2>&1 &`

## Writing Good Issues

The better your issue specification, the better the autonomous execution:

**Good issue:**
```markdown
## What
Add user avatar upload to profile page

## Requirements
- Accept PNG/JPG under 2MB
- Crop to square
- Store in /avatars/{user_id}.jpg
- Update user.avatar_url in database

## Files to change
- src/pages/profile.tsx
- src/api/upload.ts
- src/db/users.ts
```

## Related Projects

- **Ralph Loop UI** (bentossell/ralph-loop-ui) - Minimal task planner UI that reads GitHub issues and shows live loop status
- Inspired by Matt Pocock's autonomous loop implementation in his course-video-manager project

## Integration with Droid

Built by Droid (factory.ai), integrating GPT-5.2 codex capabilities for code generation and task execution.
