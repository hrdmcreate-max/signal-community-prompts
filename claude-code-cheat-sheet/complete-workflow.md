# Claude Code — Full Cheat Sheet (Commands, Codes & Prompts)

**Reference note:** This is a transcription supplied in this collection, not a claim that every command works in every installed version. Verify current availability with `claude --help` and `/help` in Claude Code. The source attribution and partial-section caveat below are retained.


Source: "Simple Tech Skills — Claude Code Cheat Sheet" (Jonathan Acuna / Doctor AI, "Illegal Claude Tips Part 37"). Transcribed from screenshots. 60+ commands across 2 pages.

> Note: the right-hand columns of a few screenshots (MCP Servers, Memory, Config Files, Key Settings, Key Env Vars) were partially cut off at the screen edge — those sections below are captured as far as they were legible and marked "(partial)".

---

## SLASH COMMANDS

### Session
- `/clear` — Clear conversation
- `/compact [focus]` — Compact context
- `/resume` — Resume / switch session
- `/rename [name]` — Name current session
- `/branch [name]` — Branch conversation
- `/cost` — Token usage + cache breakdown [NEW]
- `/context` — Visualize context grid
- `/diff` — Interactive diff viewer
- `/copy [N]` — Copy last (or Nth) response
- `/rewind` — Rewind / code checkpoint
- `/export` — Export conversation

### Config
- `/config` — Open settings
- `/model [model]` — Switch model
- `/fast [on|off]` — Toggle fast mode
- `/theme` — Change color theme
- `/permissions` — View / update permissions
- `/effort [level]` — low / med / high / max / auto
- `/keybindings` — Customize shortcuts
- `/terminal-setup` — Configure terminal

### Tools
- `/init` — Create CLAUDE.md
- `/memory` — Edit CLAUDE.md files
- `/mcp` — Manage MCP servers
- `/hooks` — Manage hooks
- `/skills` — List available skills
- `/agents` — Manage agents
- `/chrome` — Chrome integration

### Special
- `/btw` — Side question, no context cost
- `/plan [desc]` — Plan mode + auto-start
- `/loop [interval]` — Schedule recurring task
- `/voice` — Push-to-talk (20 languages)
- `/doctor` — Diagnose installation
- `/remote-control` — Bridge to claude.ai/code
- `/usage` — Plan limits and rate status
- `/schedule` — Cloud scheduled tasks
- `/feedback` — Submit feedback (alias `/bug`)
- `/release-notes` — Interactive version changelog

---

## WORKFLOWS & TIPS

### Plan Mode
- `Shift+Tab` — Cycle: Normal > Auto-Accept > Plan
- `--permission-mode plan` — Start in plan mode

### Thinking & Effort
- `Alt+T` — Toggle thinking on / off
- `"ultrathink"` — Max effort for current turn
- `Ctrl+O` — See thinking in verbose mode
- `/effort` — low / medium / high / max / auto

### Context Management
- `/context` — Usage + optimization tips
- `/compact [focus]` — Compress context with focus
- Auto-compact — Fires at ~95% capacity [NEW]
- 1M context — Opus 4.6 (Max / Team / Enterprise)
- CLAUDE.md — Survives compaction!

### Git Worktrees
- `--worktree name` — Isolated branch per feature
- `isolation: worktree` — Agent in its own worktree
- `sparsePaths` — Checkout only needed dirs
- `/batch` — Auto-creates worktrees

### Session Power Moves
- `claude -c` — Continue last conversation
- `claude -r "name"` — Resume by name
- `/btw question` — Side Q, no context cost

### Voice Mode
- `/voice` — Enable push-to-talk
- `Space (hold)` — Record, release to send

### Headless
- `claude -p "query"` — Non-interactive
- `--output-format` — Structured output
- `--max-budget-usd 5` — Cost cap
- `cat file | claude -p` — Pipe input

### Scheduling & Remote
- `/loop 5m msg` — Recurring task
- `/rc` — Remote control bridge [NEW]
- Auto mode denied → `/permissions` → Recent → Retry denied

---

## SKILLS & AGENTS

### Built-in Skills
- `/simplify` — Code review (3 parallel agents)
- `/batch` — Parallel changes (5-30 worktrees)
- `/debug [desc]` — Troubleshoot from debug log
- `/loop [interval]` — Recurring scheduled task
- `/claude-api` — Load API + SDK reference

### Custom Skill Locations
- `.claude/skills/<n>/` — Project skills
- `~/.claude/skills/<n>/` — Personal skills

### Skill Frontmatter
- `description` — Auto-invocation trigger
- `allowed-tools` — Skip permission prompts
- `model` — Override model for skill
- `effort` — Override effort level
- `paths: [globs]` — Path-specific (YAML list)
- `context: fork` — Run in subagent
- `$ARGUMENTS` — User input placeholder
- `$(CLAUDE_SKILL_DIR)` — Skill's own directory
- `` !`cmd` `` — Dynamic context injection
- `plugin bin/` — Ship executables for Bash tool [NEW]

### Agents
- Explore — Fast read-only (Haiku)
- Plan — planning agent
- General — all tools, complex tasks
- Bash — Terminal, separate context

### Agent Frontmatter
- `permissionMode` — default / acceptEdits / plan / dontAsk
- `isolation: worktree` — Run in own worktree
- `memory` — user / project / local
- `background: true` — Background task
- `initialPrompt` — Auto-submit first turn
- `handMessage` — Resume agents
- `subagent-name` — Mention named subagents [NEW]

---

## MCP SERVERS (partial — right column clipped)

- Add server: `--transport http | stdio | sse`
- Scopes: Local (`~/…`), Project, User (`~/.claude/…`)
- Manage: `/mcp`, `claude mcp list`, `claude mcp add …`
- `maxResults` override [NEW]

## MEMORY & FILES (partial — right column clipped)

- CLAUDE.md locations: `./CLAUDE.md`, `~/.claude/…`, `/etc/claude/…`
- Rules & imports: `.claude/rules…`, `~/.claude/…`, `@path/to/file`
- Auto memory: `~/.claude/projects/…`
- `MEMORY.md` — max ~5KB

## CONFIG & FILES (partial — right column clipped)

- Config files: `~/.claude…`, `.claude/settings…`, `.mcp.json`, managed-settings fragments
- Key settings: `modelOverride`, `autoMemory`, `worktree.*`, `sandbox` (fail-open), `hooks`, `permissions`, `showThinking` [NEW], forced startup hooks [NEW]

## KEY ENV VARS (partial — right column clipped)

- `ANTHROPIC_API_KEY`
- `ANTHROPIC_MODEL`
- `CLAUDE_…_EFFORT` (low / medium / high)
- `MAX_THINKING_…`
- `CLAUDE_CODE_…` (streaming / watch)
- `MCP_CONNECTION_…`

---
