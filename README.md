# zdev-skill

Agent skill for [zdev](https://github.com/5hanth/zdev) — multi-agent worktree development environment.

## What is this?

This skill teaches AI coding agents (Claude Code, Clawdbot, etc.) how to use `zdev` for managing isolated development environments with git worktrees, automatic port allocation, and public preview URLs.

## Installation

### Claude Code

```bash
npx add-skill Workstellar-ApS/zdev-skill
```

Then in Claude Code:
```
/zdev
```

### Clawdbot

Add to your Clawdbot skills directory:
```bash
git clone https://github.com/Workstellar-ApS/zdev-skill ~/.clawdbot/skills/zdev
```

### Other Agents

Copy the contents of [SKILL.md](./SKILL.md) into your agent's system prompt or context.

## Usage

Once installed, prompt your agent:

```
Use zdev to create a new TanStack Start project called my-app with Convex backend.
```

```
Use zdev to start a worktree for add-auth feature on ./my-project
```

```
Run zdev list to show what's currently running.
```

```
Use zdev clean to remove the add-auth worktree after the PR is merged.
```

## What the Agent Learns

- `zdev create` — Scaffold new TanStack Start projects
- `zdev init` — Initialize existing projects
- `zdev start` — Create isolated worktrees with auto port allocation
- `zdev list` — Check running worktrees
- `zdev stop` — Stop servers
- `zdev clean` — Remove worktrees after PR merge
- `zdev config` — Configure Traefik for public URLs

## Requirements

- [zdev](https://github.com/5hanth/zdev) CLI installed
- [Bun](https://bun.sh) runtime

## Related

- [zdev](https://github.com/5hanth/zdev) — The CLI tool
- [Clawdbot](https://docs.clawd.bot) — AI agent platform
- [Claude Code](https://claude.ai) — Anthropic's coding agent

## License

[WTFPL](https://en.wikipedia.org/wiki/WTFPL)
