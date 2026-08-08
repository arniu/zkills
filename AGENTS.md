# AGENTS.md

## Project structure

```
skills/          public — promoted, listed in README
in-progress/     private — drafts
research/        private — external skills for study, not house style
docs/            reference docs
  skills-guide.md  comprehensive skill authoring guide
```

Skills graduate from `in-progress/` to `skills/` when ready.

Every skill in `skills/` (the **promoted** bucket) must have a linked entry in `README.md`; `in-progress/` and `research/` skills must not appear there. Adding, renaming, removing, or moving a skill updates `README.md` in the same change.

Each skill under `research/` keeps its origin — source repo and license — in a `SOURCE.md` beside its `SKILL.md`; these are study material from other repos, never to be installed or imitated as house style.

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
