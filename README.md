# The Bike Project

A high-speed cargo bike optimized for long commutes. See [alec-bike.github.io][1] for details.

## Install

Clone repository:

```sh
git clone git@github.com:alec-bike/alec-bike.github.io.git
cd alec-bike.github.io
```

> [!TIP]
> This repository uses uv to manage dependencies. See [Installing uv][2] for setup instructions.

Sync local dependencies:

```sh
uv sync
```

Install prek and mdformat:

```sh
uv tool install prek
uv tool install mdformat -w mdformat-footnote -w mdformat-gfm
```

Setup and test pre-commit hooks:

```sh
prek install
prek run -a
```

Build and preview documentation:

```sh
uv run mkdocs build
uv run mkdocs serve
```

Deploy to Github Pages:

> [!important]
> Ensure 'gh-pages' is set as default branch in GitHub Pages.

```sh
uv run mkdocs gh-deploy --force
```

[1]: https://alec-bike.github.io
[2]: https://docs.astral.sh/uv/getting-started/installation/
