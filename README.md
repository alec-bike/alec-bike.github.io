# The Bike Project

A high-speed cargo bike optimized for long commutes. See [alec-bike.github.io][1] for details.

## Install

Clone repository:

```sh
git clone git@github.com:alec-bike/alec-bike.github.io.git
cd alec-bike.github.io
```

> [!TIP]
> This repository uses mdbook for documentation. See [mdbook][2] for setup instructions.

Build and preview documentation:

```sh
mdbook build -o
```

Deploy to Github Pages:

> [!NOTE]
> Ensure 'gh-pages' is set as default branch in GitHub Pages.

```sh
uv run mkdocs gh-deploy --force
```

[1]: https://alec-bike.github.io
[2]: https://rust-lang.github.io/mdBook/guide/installation.html
