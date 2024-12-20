# Bike Project

## Setup

```zsh
# install uv -> https://docs.astral.sh/uv
# add documentation package
uv init
uv add mkdocs-material --dev
 
# build and test locally
uv run mkdocs build
uv run mkdocs serve
 
# deploy to github
# set 'gh-pages' as default branch in GitHub Pages
uv run mkdocs gh-deploy --force
```
