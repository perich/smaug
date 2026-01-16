# Ralph Loop UI

**Repo:** bentossell/ralph-loop-ui
**Language:** TypeScript
**Stars:** 44
**URL:** https://github.com/bentossell/ralph-loop-ui

Minimal task planner UI that reads GitHub issues and shows live loop status.

Built by Droid (factory.ai) as a companion tool to the agent-loop system.

## Setup

### 1. Install dependencies

```bash
npm install
```

### 2. Create `.env.local`

```
AGENT_LOOP_REPO="owner/repo"
AGENT_LOOP_TOKEN="<github_token_with_repo_scope>"
```

### 3. Run locally

```bash
npm run dev
```

Open `http://localhost:3000`

## Deploy

Deploy on Vercel and set environment variables:
- `AGENT_LOOP_REPO`
- `AGENT_LOOP_TOKEN`

## Features

- Real-time loop status visualization
- GitHub issue integration
- Task planning interface
- Live progress tracking

## Related Projects

- **Agent Loop** (bentossell/agent-loop) - The core autonomous execution system that this UI monitors
- Used alongside agent-loop for complete autonomous task execution workflow
