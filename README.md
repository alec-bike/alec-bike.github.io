# The Bike Project

A high-speed electric cargo bike refined for long commutes.

See [alec-bike.github.io](https://alec-bike.github.io) for details.

## Install

Clone repository:

```sh
git clone git@github.com:alec-bike/alec-bike.github.io.git
cd alec-bike.github.io
```

Sync local dependencies:

```sh
uv sync
```

> [!tip]
> Ensure pre-commit and mdformat are setup as system tools.

Install pre-commit hooks:

```sh
pre-commit install
```

Preview the documentation site:

```sh
mdformat docs
uv run mkdocs serve -o
```

Deploy to Github Pages:

> [!important]
> Ensure 'gh-pages' is set as default branch in GitHub Pages.

```sh
uv run mkdocs gh-deploy --force
```
