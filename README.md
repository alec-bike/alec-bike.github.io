# Install

```zsh
# clone git repo
git clone git@github.com:alec-bike/alec-bike.github.io.git
cd alec-bike.github.io

# add dev dependencies (documentation and lint/format)
uv add mkdocs-material mdformat-mkdocs --dev

# build documentation and test locally
uv run mkdocs serve

# deploy site to github
# note: ensure 'gh-pages' is set as default branch in GitHub Pages
uv run mkdocs gh-deploy --force
```

# Test

**Run these commands before each commit.**

```zsh
# update dependencies
uv sync
uv tree --outdated --depth 1

# run markdown lint/format
uv run mdformat docs

# build documentation
uv run mkdocs build
```
