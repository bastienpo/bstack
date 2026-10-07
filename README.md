# bstack

Bastien's personal agent-skills plugin: shared coding standards and reusable skills for Cursor, Claude Code, Codex, and other agents.

Install once; reuse across projects. `docs/` is the source of truth for long-form standards. Skills under `skills/` ship self-contained copies via `references/` so each install works offline.

## Install with the skills CLI

```bash
npx skills add bastienpo/bstack --list
npx skills add bastienpo/bstack --skill bstack-mode -g -y
npx skills add bastienpo/bstack --all
```

## Install with Claude Code marketplace

```text
/plugin marketplace add bastienpo/bstack
/plugin install bstack@bstack
```

## Cursor plugin

This repo also includes `.cursor-plugin/plugin.json` for later Cursor plugin publishing. Same plugin name: **bstack**.

## Skills

| Skill | When to use |
| --- | --- |
| `bstack-mode` | Default working style ("bstack", "/bstack") |
| `apply-code-style` | Writing or reviewing code |
| `apply-pr-norms` | Opening or reviewing PRs |
| `prove-it` | Before claiming status, numbers, or "fixed" |
| `focused-diff` | Keep changes minimal and on-task |
| `author-bstack-skill` | Add a skill to this repo |

## Layout

```
skills/<name>/SKILL.md    # recipe + frontmatter
skills/<name>/references/ # detail that ships with the skill
docs/                     # shared standards (edit here first)
.claude-plugin/           # Claude marketplace + plugin manifest
.cursor-plugin/           # Cursor plugin manifest
AGENTS.md                 # how agents should change this repo
```

When you change a standard in `docs/`, refresh matching copies under `skills/*/references/`.

## License

MIT — Copyright (c) Bastien
