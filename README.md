# The Bike Project

Documentation repository for The Bike Project.

## Installation

Clone repository:

```sh
git clone git@github.com:alec-bike/alec-bike.github.io.git
cd alec-bike.github.io
```

> [!TIP]
> This repository uses mdbook for documentation. See [mdbook][1] for setup instructions.

Build and preview documentation:

```sh
mdbook build -o
```

Deployment to Github Pages is done by the `mdbook.yaml` workflow. Documentation is published to [alec-bike.github.io][2].

> [!NOTE]
> Ensure 'gh-pages' is set as default branch in GitHub Pages.

[1]: https://rust-lang.github.io/mdBook/guide/installation.html
[2]: https://alec-bike.github.io
