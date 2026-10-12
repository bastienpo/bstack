# bstack

Shared, tool-agnostic agent standards for all my agents.

- `skills/`: one folder per skill, each with a `SKILL.md` (frontmatter `name` and `description`). Empty for now.
- `docs/`: global reference material any agent or human can read.
- `AGENTS.md`: entry point for agents that read the `AGENTS.md` convention.

Install skills into any supported agent (Claude Code, Cursor, Codex, and others) with:

```
npx skills add bastienpo/bstack
```
