# Docs

Global standards and playbooks reused across Bastien's agents and repos. Edit here first; then copy into `skills/*/references/` so installs stay current.

| Doc | Purpose |
| --- | --- |
| [code-style.md](./code-style.md) | Default coding conventions |
| [pr-review.md](./pr-review.md) | PR shape and review expectations |
| [working-agreements.md](./working-agreements.md) | Default agent working style (bstack-mode) |

## How to update

1. Change the doc in `docs/`.
2. Copy the same file into every skill `references/` that depends on it.
3. Bump plugin version in `.claude-plugin/plugin.json` and `.cursor-plugin/plugin.json` when cutting a release.
4. Consumers run `npx skills update` (or reinstall).
