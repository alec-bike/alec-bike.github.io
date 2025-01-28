# Installation

```bash
# clone git repo
git clone git@github.com:alec-bike/alec-bike.github.io.git
cd alec-bike.github.io

# ensure `uv` is installed and up to date
uv self update

# add dev dependencies (documentation and lint/format)
uv add mkdocs-material mdformat-mkdocs --dev

# build documentation and test locally
uv run mkdocs serve

# deploy site to github
# note: ensure 'gh-pages' is default branch for GitHub Pages
uv run mkdocs gh-deploy --force
```

## Test

**Run these commands before each commit.**

```bash
# update dependencies
uv sync

# run markdown lint/format
uv run mdformat docs

# build documentation
uv run mkdocs build
```
