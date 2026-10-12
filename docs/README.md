# Docs

Global standards and playbooks reused across Bastien's agents and repos. Skills in `skills/` link here instead of duplicating content.

| Doc | Purpose |
| --- | --- |
| [code-style.md](./code-style.md) | Default coding conventions |
| [pr-review.md](./pr-review.md) | PR shape and review expectations |
| [working-agreements.md](./working-agreements.md) | Default agent working style |

## How to update

1. Change the doc in `docs/`.
2. Copy the same file into every skill `references/` that depends on it.
4. Consumers run `npx skills update` (or reinstall).
