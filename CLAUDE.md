# CLAUDE.md

## Project structure

```
skills/        public — linked in README
personal/      private — my setup
in-progress/   private — drafts
deprecated/    private — dead
```

Skills are in `in-progress/` while drafting, then moved to `skills/` when ready.

## Development workflow

- Test outputs go to `.claude/workspaces/`
- Use `isolation: "worktree"` for subagent testing to keep the working tree clean
