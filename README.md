# Project Starter

A minimal template for any language or framework. Ships pre-configured with formatting enforcement, pre-commit hooks, and CI.

## Getting Started

Create a new repository from this template on GitHub using [this link](https://github.com/new?template_name=project-starter&template_owner=threeal), or clone it locally and point it at your own remote.

## Setup

Install [Lefthook](https://lefthook.dev/) and [dprint](https://dprint.dev/), then register the pre-commit hook:

```sh
lefthook install
```

## Customizing

Replace or extend the template files to fit your project:

- **`.github/workflows/ci.yaml`** — Extend or replace the CI workflow.
- **`.github/dependabot.yaml`** — Adjust update frequency or add more package ecosystems.
- **`CLAUDE.md`** — Replace with guidance specific to your project.
- **`dprint.json`** — Add or remove dprint plugins for your language.
- **`lefthook.yaml`** — Add more pre-commit checks or other Git hooks.
- **`LICENSE`** — Replace with your preferred license, or keep the [Unlicense](https://unlicense.org/).
- **`README.md`** — Replace with a description of your project.

## Development

Before committing, run the pre-commit hook to fix formatting:

```sh
lefthook run pre-commit
```

If any file changes during the run, re-stage the changed files and retry. The hook also runs automatically on each `git commit` — if it fails, re-stage the changed files and commit again.

After committing, push to `main` or open a pull request from another branch — CI will run the pre-commit hook across all files.

## Language-Specific Templates

For a more opinionated starting point in a specific language or framework:

- **[Action Starter](https://github.com/threeal/action-starter)** — JavaScript GitHub Action projects.
- **[C++ Starter](https://github.com/threeal/cpp-starter)** — C++ projects.
- **[CMake Starter](https://github.com/threeal/cmake-starter)** — CMake projects.
- **[Composite Action Starter](https://github.com/threeal/composite-action-starter)** — Composite GitHub Action projects.
- **[Discord Bot Starter](https://github.com/threeal/discord-bot-starter)** — Discord bot projects.
- **[Node.js Starter](https://github.com/threeal/nodejs-starter)** — Node.js projects.
- **[Python Starter](https://github.com/threeal/python-starter)** — Python projects.
