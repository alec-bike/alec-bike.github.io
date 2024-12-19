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

# build and start server on http://127.0.0.1:8000
uv run mkdocs build
uv run mkdocs serve
```
