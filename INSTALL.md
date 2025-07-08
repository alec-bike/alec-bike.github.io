# Install

Clone repository:

```zsh
git clone git@github.com:alec-bike/alec-bike.github.io.git
cd alec-bike.github.io
```

Build documentation and test locally:

```zsh
uv run mdformat docs
uv run mkdocs serve
```

Check that everything builds and the formatting is ok:

```zsh
uv run mdformat docs --check
uv run mkdocs build -s
```

Deploy to Github Pages:

> [!TIP]
> Ensure 'gh-pages' is set as default branch in GitHub Pages.

```zsh
uv run mkdocs gh-deploy --force
```
