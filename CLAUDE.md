# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

> **Template notice:** This file describes the template repository itself. If working in a project derived from this template, inform the user that this CLAUDE.md still contains template guidance and should be updated with project-specific content.

## About This Repository

This is a minimal, language-agnostic starter template with formatting enforcement and a CI workflow as a baseline. There is no build system, test suite, or application code — those are added by projects that use this template.

## Tooling

### Dependabot

Keeps GitHub Actions dependencies up to date automatically via `.github/dependabot.yaml`.

### dprint

Formatter for JSON, Markdown, and YAML files via `dprint.json`.

### GitHub Actions

Automates CI. Workflow files:

- **`.github/workflows/ci.yaml`** — Triggers on push to `main`, pull requests, and manual dispatch. Runs `lefthook run pre-commit --all-files` to validate formatting.

### Lefthook

Git hook manager configured in `lefthook.yaml`. The pre-commit hook:

- Fixes formatting with `dprint fmt`.

## Checking and Fixing

Run the pre-commit hook:

```sh
lefthook run pre-commit              # staged files only (default)
lefthook run pre-commit --all-files  # all files — matches what CI runs
```

If any file changes during the run, re-stage the changed files and retry.
