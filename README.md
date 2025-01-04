# Bike Project

## Setup

```zsh
# install uv from docs.astral.sh/uv
# add documentation and linter packages
uv init
uv add mkdocs-material mdformat-mkdocs --dev

# run markdown linter
uv run mdformat docs

# build and test locally
uv run mkdocs serve

# deploy to github
# set 'gh-pages' as default branch in GitHub Pages
uv run mkdocs gh-deploy --force
```
