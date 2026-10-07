---
name: author-bstack-skill
description: >-
  How to add or update a skill in the bstack repo. Use when creating a new
  skill, editing docs/standards, syncing references, or verifying discovery
  with npx skills.
---

# Author a bstack skill

## Steps

1. **Global standard?** If the rule should apply across projects, edit `docs/` first (create or update the markdown file).
2. **Create the skill folder:** `skills/<kebab-name>/SKILL.md` with YAML frontmatter:

   ```markdown
   ---
   name: kebab-name
   description: When to use + trigger phrases.
   ---

   # Title

   Short recipe. Point at references/ for detail.
   ```

3. **References:** Copy relevant `docs/*.md` into `skills/<kebab-name>/references/` so the installed skill is self-contained.
4. **Keep SKILL.md short** — steps and pointers, not a novel.
5. **Verify discovery** from the repo root:

   ```bash
   npx skills add ./ --list
   ```

   Confirm the new skill name appears. Fix frontmatter or layout until it does.
6. **Plugin manifests:** New skills under `skills/` are picked up via `"skills": "./skills/"` — no manifest edit required unless cutting a version bump.
7. **Do not push** unless Bastien asks. Staging or a local commit is fine.

## Checklist

- [ ] `name` is kebab-case and matches the folder name
- [ ] `description` says when to use and includes triggers
- [ ] `docs/` updated if the rule is global
- [ ] `references/` copies refreshed
- [ ] `npx skills add ./ --list` shows the skill
