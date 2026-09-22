# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

> **Template notice:** This file describes the template repository itself. If working in a project derived from this template, inform the user that this CLAUDE.md still contains template guidance and should be updated with project-specific content.

## About This Repository

A minimal, language-agnostic starter template with formatting enforcement and a CI workflow baseline. No build system, test suite, or application code — those are added by projects that use this template.

## Non-Obvious Rules

- `.gitignore` ignores all dotfiles/dotdirs by default (`.*`), except `.github/` — a new dotfile or dotdir needs an explicit `!` exception or it silently won't be tracked.
- `lefthook run pre-commit --all-files` auto-fixes formatting, and `fail_on_changes` fails the run if anything changed. Without `--all-files` the job is skipped whenever nothing is staged. Report the failure and leave the fixes for the user to review and re-stage.

## Config Map

- Format — `dprint.json`
- Git hooks — `lefthook.yaml`
- CI — `.github/workflows/ci.yaml`
- Dependency updates — `.github/dependabot.yaml`

## Checking and Fixing

```sh
lefthook run pre-commit --all-files
```
