# AGENTS.md

Guidance for any coding agent working in this repository (**bstack**). Tool-agnostic: no vendor-specific config lives here.

## Layout

```
skills/<name>/SKILL.md   # one folder per skill; frontmatter needs `name` and `description`
docs/                    # shared standards, readable by any agent or human
```

## Rules

- Keep everything plain Markdown so it works with any agent.
- New skills go in `skills/<kebab-case-name>/SKILL.md`; put long reference material in `docs/` and link to it.
- Check a skill is discoverable with `npx skills add ./ --list`.
