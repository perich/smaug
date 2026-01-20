# Try - Fresh Directories for Every Vibe

Quickly manage and navigate experiment directories with fuzzy search and smart sorting.

**Repository:** [tobi/try](https://github.com/tobi/try)
**Stars:** 2903
**Language:** Shell (Ruby)

## What it does

A one-file Ruby script that solves the problem of scattered test directories. Instead of having 50 directories named `test`, `test2`, `new-test`, `actually-working-test` everywhere, try gives you:

- **Centralized location:** All experiments in one place (default: `~/src/tries`)
- **Fuzzy search:** Smart matching like `rds` → `redis-server`
- **Auto-dating:** Creates directories like `2025-08-17-redis-experiment`
- **Time-aware sorting:** Recently used projects float to the top
- **Zero config:** Just one Ruby file, no dependencies

## Installation

### Via RubyGems (Recommended)

```bash
gem install try-cli
eval "$(try init)"  # Bash/Zsh
eval (try init | string collect)  # Fish
```

### Manual

```bash
curl -sL https://raw.githubusercontent.com/tobi/try/refs/heads/main/try.rb > ~/.local/try.rb
chmod +x ~/.local/try.rb
echo 'eval "$(ruby ~/.local/try.rb init ~/src/tries)"' >> ~/.zshrc
```

## Usage

```bash
try                                    # Browse all experiments
try redis                              # Jump to redis experiment or create
try new api                            # Create with custom name
try . [name]                           # Create worktree from current repo
try ./path/to/repo [name]              # Use another repo as worktree source
try clone https://github.com/user/repo  # Clone into dated directory
try --help                             # Show all options
```

## Features

### Smart Fuzzy Search
- Not substring matching; actual smart search
- `connpool` matches `connection-pool`
- Recent projects score higher
- Shorter names win on equal matches

### Time-Aware
- Shows how long ago you touched each project
- Perfect for "what was I working on yesterday?"
- Recently accessed float to top

### Pretty TUI
- Clean, minimal interface
- Highlights matches as you type
- Shows scores so you understand ranking
- Dark mode by default

### Organized Chaos
- Auto-prefixes with dates: `2025-08-17-your-idea`
- Configurable via `TRY_PATH` environment variable
- Skip date prompt by pre-typing a name

## Performance

Highly optimized with Ruby's profiler:
- Opens 2000 directories in 54ms
- Faster than the C version
- Generated with agent-assisted optimization

## Configuration

```bash
# Use custom experiments directory
export TRY_PATH=~/experiments
try redis
```

## Git integration

Supports git worktrees:
- Inside Git repo: creates detached HEAD worktree
- Outside repo: simply creates directory
- Clone shorthand: `try https://github.com/user/repo.git`

## Use case

Perfect for developers who constantly create small experiments, POCs, and learning projects. Eliminates friction of file organization while keeping projects organized and findable.
