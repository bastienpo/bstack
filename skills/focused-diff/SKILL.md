---
name: focused-diff
description: >-
  Keep changes minimal and on-task. No drive-by refactors, unrelated formatting,
  or scope creep. Use when editing code, reviewing a diff, or when asked to
  keep the PR/change small.
---

# Focused diff

Ship the smallest change that completes the asked task.

## Rules

1. Touch only files required for the task.
2. No drive-by refactors, renames, or style sweeps mixed into feature work.
3. Do not "while I'm here" fix unrelated issues — note them as follow-ups instead.
4. If unrelated work is necessary, split it into a separate commit or PR.
5. Prefer updating an existing function over introducing parallel helpers.
6. Before finishing, re-read the diff and drop anything that is not on-task.

## When tempted to expand

- Ask: does this line help the stated goal?
- If no, revert it or park it for later.
