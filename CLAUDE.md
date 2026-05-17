# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

> **Template notice:** This file describes the template repository itself. If you've created a project from this template, replace this content with guidance specific to your project.

## About This Repository

This is a minimal, language-agnostic GitHub repository template. It includes formatting enforcement and a CI workflow as a baseline — there is no build system, test suite, or application code. Those are added by projects that use this template.

## Formatting

Format all files with dprint:

```sh
dprint fmt
```

Check formatting without modifying files:

```sh
dprint check
```

dprint is configured in `dprint.jsonc` to handle JSON, Markdown, and YAML files.

## Git Hooks

Lefthook manages Git hooks (`lefthook.yaml`). The pre-commit hook runs `dprint fmt` automatically and fails the commit if formatting changes are required. Run `lefthook install` after cloning to activate the hooks.

## CI

The only CI job (`.github/workflows/ci.yaml`) validates formatting with `dprint check` on PRs and pushes to `main`.
