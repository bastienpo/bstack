# PR and review norms

Bastien's defaults for opening and reviewing pull requests.

## Shape

- One concern per PR when practical; split unrelated work.
- Title and description explain **why**, not only what.
- Prefer draft PRs until CI is green and the change is ready for review.
- Keep the diff focused; link follow-ups instead of sneaking them in.

## Ready to merge

- Required checks green.
- At least one approval (or CODEOWNERS satisfied).
- Description updated if the approach changed during review.
- No unresolved blocking comments.

## Reviewer habits

- Lead with blocking issues; then nits.
- Prefer concrete suggestions over vague preference.
- Ask for evidence when behavior claims are unclear (tests, logs, screenshots).

## Git hygiene

- Do not force-push shared branches without an explicit ask.
- Prefer rebase only when the branch is not shared, or when asked.
- Squash when the history is noisy; keep meaningful commits when they tell a story.
