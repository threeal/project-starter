# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## About This Repository

This is a language-agnostic GitHub repository template. It provides formatting enforcement and CI/CD infrastructure as a starting point for new projects. There is no build system, test suite, or application code — those are added by projects that use this template.

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

The only CI job (`.github/workflows/check.yaml`) validates formatting with `dprint check` on PRs and pushes to `main`.
