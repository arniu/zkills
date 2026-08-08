# AGENTS.md

## Project structure

```
skills/          public — promoted, listed in README
in-progress/     private — drafts
deprecated/      private — dead
docs/            reference docs
  skills-guide.md  comprehensive skill authoring guide
```

Skills graduate from `in-progress/` to `skills/` when ready.

Every skill in `skills/` (the **promoted** bucket) must have a linked entry in `README.md`; `in-progress/` and `deprecated/` skills must not appear there. Adding, renaming, removing, or moving a skill updates `README.md` and `skills/README.md` in the same change.

## Skill format

Each skill is a directory with a `SKILL.md` containing:

- **YAML frontmatter**: `name`, `description` (the only trigger mechanism)
- **Body**: instructions under 500 lines
- Optional: `evals/`, `references/`, `scripts/`, `assets/`

See `docs/skills-guide.md` for full conventions, including evals.

## Commands

```bash
# Test a skill (via /skill-creator eval framework)
```

`README.md` is the single source of install wording — don't restate install commands in skills, docs, or this file.

## Development workflow

- Test outputs go to `.claude/workspaces/`
- Use `isolation: "worktree"` for subagent testing to keep the working tree clean
