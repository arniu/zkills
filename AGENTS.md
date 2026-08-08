# AGENTS.md

## Project structure

```
skills/          public — promoted
in-progress/     private — drafts
research/        private — external skills for study
docs/            reference docs
  skills-guide.md      authoring conventions (incl. evals)
  skills-philosophy.md writing methodology
```

Skills graduate from `in-progress/` to `skills/` when their evals pass.

`README.md` lists exactly the `skills/` set — every promoted skill linked, nothing from `in-progress/` or `research/`. Adding, renaming, removing, moving, or changing a skill's description updates `README.md` in the same change. Install commands live only in `README.md`.

Each skill under `research/` is study material from another repo — read and learn from it, keep its origin (source repo and license) in a `SOURCE.md` beside its `SKILL.md`.

## Skill format

Each skill is a directory with a `SKILL.md` containing:

- **YAML frontmatter**: `name`, `description` (the only trigger mechanism)
- **Body**: instructions under 500 lines
- Optional: `evals/`, `references/`, `scripts/`, `assets/`

See `docs/skills-guide.md` for the full conventions — authoring, evals, tuning.

## Development workflow

- Test a skill via the `/skill-creator` eval framework — an installed skill, not part of this repo (workflow in `docs/skills-guide.md`)
- Test outputs go to `.claude/workspaces/`
- Use `isolation: "worktree"` for subagent testing to keep the working tree clean
