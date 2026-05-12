# Skills For AI Native

AI-native skills for Claude Code. Install, use, and build your own.

## Installation

### Prerequisites

- [Claude Code](https://claude.ai/code) CLI installed (`claude` command available in your terminal)

### Install a skill

```bash
claude add skill <path>
```

Where `<path>` is the local path to the skill directory.

Clone the repo and use `claude add skill` with the skill path:

```bash
claude add skill skills/model-thinker
```

### Verify installation

After installing, start a new Claude session and type `/` — the skill should appear in your available slash commands. Or check directly:

```bash
claude list skills
```

## Available Skills

- [model-thinker](skills/model-thinker/) — Multi-model analysis via Scott Page's The Model Thinker
  - Install: `claude add skill skills/model-thinker`
