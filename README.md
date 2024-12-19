# Bike Project

## Setup

```zsh
# install uv
curl -LsSf https://astral.sh/uv/install.sh | sh
echo "source $HOME/.cargo/env" >> ~/.zprofile
 
# clone git repo
git clone git@github.com:alec-bike/alec-bike.github.io
cd alec-bike.github.io
 
# install mkdocs-material documentation package
uv add mkdocs-material --dev
 
# build and start server on localhost:8000
uv run mkdocs build
uv run mkdocs serve
 
# deploy to github -> https://alec-bike.github.io
# note: set `gh-pages` as the Github Pages branch
uv run mkdocs gh-deploy --force
```
