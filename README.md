# yuxiaodai.github.io

Personal site built with [Quarto](https://quarto.org), deployed to GitHub Pages.

## Local preview

```sh
quarto preview
```

## Add a post

1. Create `posts/YYYY-MM-DD-slug/index.qmd` (or `index.ipynb`) with `title`, `date`,
   `description`, and `categories` in the front matter.
2. Run `quarto render` locally so results are frozen into `_freeze/`; commit `_freeze/`.
   CI never re-runs experiments.
3. Push to `main`. The workflow renders and publishes to the `gh-pages` branch.

## Content rules

- Desensitized content only: no employer, no finance framing, no job-search signals.
- Every number links to the script that produced it.

## First-time setup

1. Push this repo as `YuxiaoDai/YuxiaoDai.github.io` (public).
2. Run `quarto publish gh-pages` once locally (creates the branch), or let the workflow run.
3. Settings → Pages → Source: deploy from branch `gh-pages` / root.
