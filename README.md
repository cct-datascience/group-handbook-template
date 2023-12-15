# group-handbook-template

<!-- badges: start -->

[![Project Status: Concept -- Minimal or no implementation has been done yet, or the repository is only intended to be a limited example, demo, or proof-of-concept.](https://www.repostatus.org/badges/latest/concept.svg)](https://www.repostatus.org/#concept)

<!-- badges: end -->

This is a work-in-progress, but will eventually be a template repo that contains a skeleton of a lab group handbook (much like the one described by [Tendler et al., 2023](https://doi.org/10.7554/eLife.88853)).

## Things to edit

I'll turn this into instructions later, but here's a running list of things you'll need to edit after using this template:

-   Everything in `_variables.yml`

-   `author:` in `_quarto.yml` (can't do lists with shortcodes)

-   `cover.png` and `cover-image` in `_quarto.yml` if you want a lab logo.

-   `repo_url` in `_quarto.yml`

## To publish

You only have to do this once.

Run `quarto publish gh-pages` in the terminal to create `_publish.yml`.
Commit and push `_publish.yml` and from then on the book should automatically re-render when changes are pushed to the GitHub repo.
