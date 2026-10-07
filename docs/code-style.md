# Code style

Bastien's default coding conventions. Prefer these unless the local file or project already has a stricter rule.

## Defaults

- Prefer clear names over clever abbreviations.
- Keep functions small and single-purpose.
- Avoid comments that restate the code; encode intent in names and structure.
- Match the style already used in the file and neighboring modules.
- Do not invent APIs or dependencies without an explicit ask.
- Prefer early returns over deep nesting.
- Handle errors explicitly; do not swallow them.
- Leave the codebase easier to change than you found it — without drive-by refactors.

## Diffs

- Change only what the task requires.
- No unrelated formatting sweeps mixed into feature work.
- If a rename or cleanup is needed, do it in a separate commit or PR when practical.

## Languages

Add language-specific sections (TypeScript, Python, Go, …) as you need them. Until then, follow the project linter/formatter and the defaults above.
