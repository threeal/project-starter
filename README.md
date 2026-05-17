# Project Starter

A minimal GitHub repository template with formatting enforcement and CI/CD ready to go, for any language or framework.

## What's Included

- **Formatting** with [dprint](https://dprint.dev/) — supports JSON, Markdown, and YAML out of the box
- **Pre-commit hooks** with [Lefthook](https://lefthook.dev/) — auto-formats files before each commit
- **Dependabot** — keeps GitHub Actions dependencies up to date automatically
- **CI workflow** — validates formatting on every pull request and push to `main`

## Getting Started

1. [Create a new repository](https://github.com/new?template_name=project-starter&template_owner=threeal) from this template, or clone it directly.
2. Install [Lefthook](https://lefthook.dev/install/) and run `lefthook install` to activate the pre-commit hook.
3. Replace the [`LICENSE`](./LICENSE) file with your preferred license, or keep it to keep the project [unlicensed](https://unlicense.org/).
4. Modify the template files to fit your project.

## Customizing

Each config file is a starting point — modify it to fit your needs:

- `dprint.jsonc` — add or remove dprint plugins for your language
- `lefthook.yaml` — add more pre-commit checks or other Git hooks
- `.github/workflows/ci.yaml` — extend or replace the CI workflow
- `.github/dependabot.yaml` — adjust update frequency or add more package ecosystems
- `CLAUDE.md` — replace with guidance for your project's structure, tools, and development workflow (for Claude Code)

## Language-Specific Templates

For a more opinionated starting point in a specific language or framework:

- [Action Starter](https://github.com/threeal/action-starter)
- [C++ Starter](https://github.com/threeal/cpp-starter)
- [CMake Starter](https://github.com/threeal/cmake-starter)
- [Composite Action Starter](https://github.com/threeal/composite-action-starter)
- [Discord Bot Starter](https://github.com/threeal/discord-bot-starter)
- [Node.js Starter](https://github.com/threeal/nodejs-starter)
- [Python Starter](https://github.com/threeal/python-starter)
