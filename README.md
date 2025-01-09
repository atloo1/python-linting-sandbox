# python-linting-sandbox

[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/atloo1/python-linting-sandbox/ci.yaml)](https://github.com/atloo1/python-linting-sandbox/actions/workflows/ci.yaml?query=branch%3Amain)
[![Dynamic TOML Badge](https://img.shields.io/badge/dynamic/toml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fatloo1%2Fpython-linting-sandbox%2Frefs%2Fheads%2Fmain%2Fpyproject.toml&query=%24.project.requires-python&label=python)](https://github.com/atloo1/python-linting-sandbox/blob/main/pyproject.toml)
[![Dynamic TOML Badge](https://img.shields.io/badge/dynamic/toml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fatloo1%2Fpython-linting-sandbox%2Frefs%2Fheads%2Fmain%2Fpyproject.toml&query=%24.project.version&label=version)](https://github.com/atloo1/python-linting-sandbox/blob/main/pyproject.toml)
[![GitHub License](https://img.shields.io/github/license/atloo1/python-linting-sandbox)](https://github.com/atloo1/python-linting-sandbox/blob/main/LICENSE)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/atloo1/python-linting-sandbox)

[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
[![Renovate enabled](https://img.shields.io/badge/renovate-enabled-brightgreen.svg)](https://renovatebot.com/)
[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)

Lint anything for a Python project according to this [pyproject.toml](https://github.com/atloo1/python-linting-sandbox/blob/main/pyproject.toml) & [.pre-commit-config.yaml](https://github.com/atloo1/python-linting-sandbox/blob/main/.pre-commit-config.yaml).

## setup

- [poetry](https://python-poetry.org/docs/#installing-with-pipx) (required)
- [pyenv](https://github.com/pyenv/pyenv?tab=readme-ov-file#installation) (recommended)

```
git clone https://github.com/atloo1/python-linting-sandbox.git
cd python-linting-sandbox/
pyenv install 3.9 --skip-existing
pyenv local 3.9
poetry install
poetry run pre-commit install
```

## run

```
touch python_linting_sandbox/<file>
poetry run pre-commit run --all-files
```
