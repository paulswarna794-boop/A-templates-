# agentic-template

[![Build](https://github.com/greynewell/agentic-template/actions/workflows/build.yml/badge.svg)](https://github.com/greynewell/agentic-template/actions)
[![License](https://img.shields.io/badge/license-MIT-blue)](./LICENSE)

A starter template for AI-first development. Scaffolds `AGENTS.md`, `CLAUDE.md`, `CHANGELOG`, and `README` so coding agents like Claude Code, Cursor, and Copilot have the right context from day one.

## Quick Start

Click **[Use this template](https://github.com/greynewell/agentic-template/generate)** on GitHub, or:

```bash
gh repo create my-project --template greynewell/agentic-template --clone
```

## What's Included

| File | Purpose |
|------|---------|
| `README.md` | Structured project README with badges, architecture diagram, and contribution guide |
| `AGENTS.md` | Guidelines and hard rules for AI coding agents |
| `CLAUDE.md` | Entry point for Claude Code — references `AGENTS.md` |
| `CHANGELOG.md` | [Keep a Changelog](https://keepachangelog.com) format with `[Unreleased]` section |
| `.claude/settings.json` | Sandbox settings for Claude Code — auto-sandboxes bash commands |
| `.github/workflows/build.yml` | CI that validates project structure on every push and PR |

## How It Works

**`CLAUDE.md`** is the first file Claude Code reads when it enters your project. It points to **`AGENTS.md`**, which contains the rules any AI coding agent should follow — changelog discipline, commit conventions, code style expectations, and PR requirements.

The **build workflow** enforces the structure: required files must exist, the changelog must have an `[Unreleased]` section, and `CLAUDE.md` must reference `AGENTS.md`. This keeps agents and humans aligned from the first commit.

## Customizing

After creating your repo from this template:

1. **`README.md`** — Replace the placeholder sections with your project's name, description, architecture, and build commands
2. **`AGENTS.md`** — Add project-specific rules (language conventions, test requirements, deployment constraints)
3. **`CHANGELOG.md`** — Start logging changes under `[Unreleased]`
4. **`.github/workflows/build.yml`** — Extend with your actual build, test, and deploy steps

## README Template

The included README follows a consistent structure designed for scannability:

```
# project-name         <- Name
[badges]               <- Status at a glance
[one-liner]            <- What it does

## Quick Start          <- How to use it in 3 commands
## Architecture         <- Mermaid diagram + explanation
## Features             <- Bullet list
## Development          <- Prerequisites, build, test
## Contributing         <- Fork/branch/PR workflow
## Roadmap              <- Link to project board
## Documentation        <- Links to docs
## License              <- License
[footer]               <- Site link, author
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

[MIT](./LICENSE)

---

Created by [Grey Newell](https://greynewell.com)
