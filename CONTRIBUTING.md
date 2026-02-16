# Contributing

If you want to contribute on this project here are some instructions to start a development environment.

## How to start developing on this project

### Installing [uv package manager](https://docs.astral.sh/uv/) and dependencies

To install [uv package manager](https://docs.astral.sh/uv/) you can either:

- install it globally by following instructions on the website.
- or via conda if a corporate environment `conda install uv`

Then to install dependencies you can use `uv sync` command.

You can also install additional dependencies for specific tasks:

- `uv sync --group dev` (to install jupyter)
- `uv sync --group tests` (to install pytest and execute test)
- `uv sync --group docs` (to install sphinx)
- `uv sync --group generator` (to install yapf)
- `uv sync --all-groups` (to install all extra dependencies)

### How to run tests ?

`uv run pytest`

### How to generate the documentation ?

> FIXME: you need to install pandoc in your computer

`uv run --group docs sphinx-build docs/ docs/_build `
