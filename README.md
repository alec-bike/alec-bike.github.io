# The Bike Project

A high-speed electric cargo bike refined for long commutes.

See [alec-bike.github.io](https://alec-bike.github.io) for details.

## Install

Clone repository:

```zsh
git clone git@github.com:alec-bike/alec-bike.github.io.git
cd alec-bike.github.io
```

Build documentation and test locally:

```zsh
mdformat docs
uv run mkdocs serve
```

Check that everything builds and the formatting is ok:

```zsh
mdformat docs --check
uv run mkdocs build -s
```

Deploy to Github Pages:

> [!important]
> Ensure 'gh-pages' is set as default branch in GitHub Pages.

```zsh
uv run mkdocs gh-deploy --force
```
