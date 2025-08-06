# The Bike Project

A high-speed electric cargo bike refined for long commutes.

See [alec-bike.github.io](https://alec-bike.github.io) for details.

## Install

Clone repository:

```sh
git clone git@github.com:alec-bike/alec-bike.github.io.git
cd alec-bike.github.io
```

> [!tip]
> Ensure pre-commit, mdformat and mkdocs are setup as system tools.

Install pre-commit hooks:

```sh
pre-commit install
```

Preview website:

```sh
mdformat docs --check
mkdocs serve -o
```

Deploy to Github Pages:

> [!tip]
> Ensure 'gh-pages' is set as default branch in GitHub Pages.

```sh
mkdocs gh-deploy --force
```
