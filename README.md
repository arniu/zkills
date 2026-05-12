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

**Public skills** (shared with the community):

```bash
claude add skill skills/model-thinker
```

**Personal skills** (your private utilities):

```bash
claude add skill personal/caveman
```

### Verify installation

After installing, start a new Claude session and type `/` — the skill should appear in your available slash commands. Or check directly:

```bash
claude list skills
```

## Available Skills

### Public (`skills/`)

- [model-thinker](skills/model-thinker/) — Multi-model analysis via Scott Page's The Model Thinker
  - Install: `claude add skill skills/model-thinker`

### Personal (`personal/`)

- [caveman](personal/caveman/) — Ultra-compressed communication mode
  - Install: `claude add skill personal/caveman`
