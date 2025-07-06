# Project Starter

A minimalist template for starting a new project on [GitHub](https://github.com/).

This template provides a basic setup for any kind of project on GitHub, independent of the project’s language or framework, with built-in support for formatting and continuous integration.

## Key Features

- Supports formatting with [dprint](https://dprint.dev/).
- Fixes formatting during pre-commit hooks using [Lefthook](https://lefthook.dev/).
- Preconfigured workflows for [Dependabot](https://docs.github.com/en/code-security/dependabot) and [GitHub Actions](https://github.com/features/actions).

## Usage

This guide explains how to use this template to start a new project on GitHub.

### Create a New Project

Follow [this link](https://github.com/new?template_name=project-starter&template_owner=threeal) to create a new project based on this template. For more information about creating a repository from a template on GitHub, refer to [this documentation](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template).

Next, clone the project you just created to your local machine. For more information, refer to [this documentation](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository). Alternatively, you can skip creating a new project and directly clone this repository to begin using the template.

### Set Up Tools

#### Set Up Git Hooks

This template uses [Lefthook](https://lefthook.dev/) to manage Git hooks, especially the pre-commit hook. If you don't want to use Git hooks, you can skip this step.

If Lefthook is not installed on your system, install it by following [this documentation](https://lefthook.dev/installation/index.html). Then, install the Git hooks by running the following command:

```sh
lefthook install
```

After that, each commit to the project will trigger hooks that check for formatting. This ensures that committed files follow the specified rules. For more information on Lefthook and how it manages hooks, refer to [this documentation](https://lefthook.dev/usage/index.html).

### Developing the Project

#### Choose a License

By default, this template is [unlicensed](https://unlicense.org/). Before modifying the template, it is recommended to replace the [`LICENSE`](./LICENSE) file with the license you want to use for your project. For more information about licensing a repository, refer to [this documentation](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository).

Alternatively, you can remove the `LICENSE` file or leave it as is to keep the project unlicensed.

### Writing the Project

Modify each file in this template according to your needs. Refer to each file for more information about what to update.

Alternatively, if you're looking for a language- or framework-specific template, you can refer to the following list:

- [Node.js Starter](https://github.com/threeal/nodejs-starter): for starting a new [Node.js](https://nodejs.org/en) project.
  - [Action Starter](https://github.com/threeal/action-starter): for starting a new [GitHub Action](https://github.com/features/actions) project.
  - [Discord Bot Starter](https://github.com/threeal/discord-bot-starter): for starting a new [Discord](https://discord.com/) bot project.
- [Python Starter](https://github.com/threeal/python-starter): for starting a new [Python](https://www.python.org/) project.
- [C++ Starter](https://github.com/threeal/cpp-starter): for starting a new [C++](https://isocpp.org/) project.
- [CMake Starter](https://github.com/threeal/cmake-starter/): for starting a new [CMake](https://cmake.org/) project.
- [Composite Action Starter](https://github.com/threeal/composite-action-starter): for starting a new composite [GitHub Action](https://github.com/features/actions) project.

#### Push the Changes

After making your changes, commit them and push to GitHub. Each push to the `main` branch will trigger a GitHub Actions workflow for continuous integration. For more details on GitHub Actions workflows, refer to [this documentation](https://docs.github.com/en/actions/about-github-actions/understanding-github-actions).

Instead of pushing directly to the `main` branch, it is recommended to push to a separate branch and then create a pull request to merge into `main`. This allows changes to be reviewed and validated by GitHub Actions before merging. For more information on pull requests, refer to [this documentation](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).

### What's Next?

Next, you can release the project or share it with others. You can also create a new issue if you find something wrong in this template or open a new pull request if you have a suggestion for improvement.
