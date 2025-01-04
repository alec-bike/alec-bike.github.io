# Installation

## Setup

```bash
# install uv from `docs.astral.sh/uv`
# add dev dependencies (documentation and linter)
uv init
uv add mkdocs-material mdformat-mkdocs --dev

# run markdown linter on all documents
uv run mdformat docs

# build and test locally
uv run mkdocs serve
```

## Deploy

```bash
# deploy to github
# ensure 'gh-pages' is default branch in GitHub Pages
uv run mkdocs gh-deploy --force
```
