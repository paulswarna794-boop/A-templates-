# AGENTS.md

Guidelines for AI coding agents working in this repository.

## Hard Rules

1. **Keep the CHANGELOG up to date.** Every user-facing change — features, fixes, breaking changes, deprecations — must have an entry in `CHANGELOG.md` under the `[Unreleased]` section before the relevant PR is merged. Do not skip this step. If a change touches behavior, it gets a changelog entry.

2. **Follow the existing code style.** Match the patterns, naming conventions, and structure already present in the codebase. Do not introduce new formatting rules, linters, or style changes unless explicitly asked.

3. **Do not create files unless necessary.** Prefer editing existing files. Do not generate documentation, READMEs, or config files unless the task requires it.

4. **Run tests before committing.** If the project has a test suite, run it and confirm it passes before staging changes.

5. **Keep commits atomic.** Each commit should represent one logical change. Do not bundle unrelated changes.

6. **Do not modify CHANGELOG structure.** Use the existing format. Add entries under `[Unreleased]` in the correct sub-section (`Added`, `Changed`, `Fixed`, `Removed`). Never edit entries under released version headers.

## CHANGELOG Format

Follow [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

```markdown
## [Unreleased]

### Added
- New features go here

### Changed
- Changes to existing functionality

### Fixed
- Bug fixes

### Removed
- Removed features or deprecated code
```

When a version is released, move all `[Unreleased]` entries under a new version header with the release date:

```markdown
## [1.0.0] - 2025-01-15
```

## Commit Messages

- Use imperative mood: "Add feature" not "Added feature"
- Keep the first line under 72 characters
- Reference issue numbers when applicable

## Pull Requests

- PR title should be concise (under 72 characters)
- PR body should summarize what changed and why
- Confirm the CHANGELOG has been updated before requesting review
