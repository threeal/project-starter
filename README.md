# Project Starter

A minimal GitHub repository template with formatting enforcement and CI/CD ready to go, for any language or framework.

## Getting Started

Create a new repository from this template on GitHub using [this link](https://github.com/new?template_name=project-starter&template_owner=threeal), or clone it locally and point it at your own remote.

## Setup

Install [Lefthook](https://lefthook.dev/), then register the pre-commit hook:

```sh
lefthook install
```

## Customizing

Replace or extend the template files to fit your project:

- **`dprint.json`** — Add or remove dprint plugins for your language.
- **`lefthook.yaml`** — Add more pre-commit checks or other Git hooks.
- **`.github/workflows/ci.yaml`** — Extend or replace the CI workflow.
- **`.github/dependabot.yaml`** — Adjust update frequency or add more package ecosystems.
- **`README.md`** — Replace with a description of your project.
- **`CLAUDE.md`** — Replace with guidance specific to your project.
- **`LICENSE`** — Replace with your preferred license, or keep the [Unlicense](https://unlicense.org/).

## Development

Before committing, run the pre-commit hook to fix formatting:

```sh
lefthook run pre-commit
```

If any files change during the run, re-stage them and retry. The hook also runs automatically on each `git commit` — if it fails, fix the reported issues, re-stage, and commit again.

## CI

`.github/workflows/ci.yaml` runs `lefthook run pre-commit --all-files` on every push and pull request.

## Language-Specific Templates

For a more opinionated starting point in a specific language or framework:

- [Action Starter](https://github.com/threeal/action-starter)
- [C++ Starter](https://github.com/threeal/cpp-starter)
- [CMake Starter](https://github.com/threeal/cmake-starter)
- [Composite Action Starter](https://github.com/threeal/composite-action-starter)
- [Discord Bot Starter](https://github.com/threeal/discord-bot-starter)
- [Node.js Starter](https://github.com/threeal/nodejs-starter)
- [Python Starter](https://github.com/threeal/python-starter)
