# Install

```zsh
# clone git repo
git clone git@github.com:alec-bike/alec-bike.github.io.git
cd alec-bike.github.io

# add dev dependencies (documentation and lint/format)
uv add mkdocs-material mdformat-mkdocs mdformat-footnote --dev

# build documentation and test locally
uv run mkdocs serve

# deploy site to github
# note: ensure 'gh-pages' is set as default branch in GitHub Pages
uv run mkdocs gh-deploy --force
```

# Update

```zsh
uv sync
uv tree --outdated --depth 1
uv run mdformat docs
uv run mkdocs build
```
