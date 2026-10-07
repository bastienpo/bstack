# AGENTS.md

Guidance for coding agents working in this repository (the **bstack** plugin).

## Purpose

Installable source for Bastien's shared agent skills:

- `npx skills add bastienpo/bstack`
- Claude marketplace plugin `bstack@bstack`
- Cursor `.cursor-plugin/plugin.json`

## Layout

```
skills/{skill-name}/SKILL.md     # required
skills/{skill-name}/references/  # optional supporting docs
docs/                            # global standards (source of truth)
.claude-plugin/                  # marketplace + plugin manifests
.cursor-plugin/                  # Cursor plugin manifest
```

## Adding a skill

Prefer the `author-bstack-skill` skill. Short version:

1. If the rule is a durable standard, update `docs/` first.
2. Create `skills/{kebab-name}/SKILL.md` with YAML frontmatter:

```markdown
---
name: kebab-name
description: When to use this skill. Include trigger phrases.
---

# Title

Steps the agent should follow.
```

3. Keep `SKILL.md` short. Put detail in `references/` and tell the agent to read those files when needed.
4. Copy relevant `docs/` files into that skill's `references/`.
5. Verify: `npx skills add ./ --list` from the repo root.

## Docs vs skills

- `docs/` — human- and agent-readable standards shared across projects; not installed by the skills CLI by itself.
- `skills/*/references/` — what actually ships with an installed skill. Keep these in sync with `docs/` when you change a standard.

## Do not

- Do not push to GitHub unless Bastien explicitly asks.
- Do not invent APIs or dependencies without an explicit ask.
- Do not copy third-party skill text (e.g. pstack) into this repo; write original bstack content.
