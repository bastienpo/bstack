---
name: prove-it
description: >-
  Before reporting a status, number, path, or "fixed", run the command or check
  that proves it and quote the evidence. Use when verifying installs, tests,
  builds, counts, git state, or any claim that could be wrong.
---

# Prove it

Do not assert outcomes from memory or hope. Show the check.

## Steps

1. Identify the claim (status, number, "works", "fixed", "installed", …).
2. Run the smallest command or inspection that would falsify the claim.
3. Quote the relevant evidence (command + key output lines). Prefer facts over paraphrase.
4. If the check fails, report failure and next step — do not claim success.
5. If you cannot run a check, say so and what would prove it.

## Examples of proofs

- Tests green → paste the test command exit and summary.
- Skill listed → `npx skills add ./ --list` output including the skill name.
- File exists → path listing or read confirmation.
- PR checks → actual check status from the host, not an assumption.
