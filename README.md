# The Bike Project

A high-speed electric cargo bike optimized for long commutes. See [alec-bike.github.io][1] for details.

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
> Ensure [prek][2] and [mdformat][3] are setup as system tools.

Install pre-commit hooks:

```sh
prek install
```

Preview the documentation site:

```sh
uv run mkdocs serve
```

Deploy to Github Pages:

> [!important]
> Ensure 'gh-pages' is set as default branch in GitHub Pages.

```sh
uv run mkdocs gh-deploy --force
```

[1]: https://alec-bike.github.io
[2]: https://github.com/j178/prek
[3]: https://github.com/hukkin/mdformat
