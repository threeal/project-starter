# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

> **Template notice:** This file describes the template repository itself. If working in a project derived from this template, inform the user that this CLAUDE.md still contains template guidance and should be updated with project-specific content.

## About This Repository

This is a minimal, language-agnostic GitHub repository template. It includes formatting enforcement and a CI workflow as a baseline — there is no build system, test suite, or application code. Those are added by projects that use this template.

## Tooling

- **Dependabot** — Keeps GitHub Actions dependencies up to date automatically via `.github/dependabot.yaml`.
- **dprint** — Formatter for JSON, Markdown, and YAML files via `dprint.json`; derived templates may replace this with a language-native formatter (e.g. Prettier for Node.js).
- **Lefthook** — Git hook manager via `lefthook.yaml`.

## Checking and Fixing

Use Lefthook to run the same steps as the pre-commit hook:

```sh
lefthook run pre-commit              # staged files only (default)
lefthook run pre-commit --all-files  # all files — matches what CI runs
```

This runs `dprint fmt` to fix formatting. If any file changes during the run, it fails and shows a diff — re-stage the changed files and retry.

Individual command (manual fallback if needed): `dprint fmt`.

## CI

CI (`.github/workflows/ci.yaml`) runs on PRs and pushes to `main`. It validates the pre-commit hook with `lefthook run pre-commit --all-files`.
