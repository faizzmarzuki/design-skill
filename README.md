# design-skill

Personal Claude Code skill: **design-taste** (`SKILL.md` at repo root).

Durable UI/design judgment plus a "Current register" of live trends. The
Current register section is refreshed automatically every 2 hours by a scheduled
Claude Code cloud agent (web-sourced trend research) as a rolling PR on branch
`design-trends-auto` into `main`. The five moves and guardrails stay stable; only
the trend snapshot and its date change. Review each PR before merging.

## Local sync
This repo is cloned directly as `~/.claude/skills/design-taste/`, so:

    git -C ~/.claude/skills/design-taste pull

updates the skill Claude Code actually loads.
