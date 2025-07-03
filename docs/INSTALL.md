# Install

```zsh
# clone git repo
git clone git@github.com:alec-bike/alec-bike.github.io.git
cd alec-bike.github.io

# add dev dependencies (documentation and format)
uv add mkdocs-material mdformat-mkdocs mdformat-footnote --dev
```

# Build

```zsh
# build documentation, test locally
uv run mdformat docs
uv run mkdocs serve

# deploy site to github
# note: ensure 'gh-pages' is set as default branch in GitHub Pages
uv run mkdocs gh-deploy --force
```

# Update

```zsh
uv sync
uv tree --outdated --depth 1
uv run mdformat docs --check
uv run mkdocs build -s -q
```
