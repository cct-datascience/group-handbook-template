# group-handbook-template

<!-- badges: start -->

[![Project Status: Concept -- Minimal or no implementation has been done yet, or the repository is only intended to be a limited example, demo, or proof-of-concept.](https://www.repostatus.org/badges/latest/concept.svg)](https://www.repostatus.org/#concept)

<!-- badges: end -->

This is a work-in-progress, but will eventually be a template repo that contains a skeleton of a lab group handbook (much like the one described by [Tendler et al., 2023](https://doi.org/10.7554/eLife.88853)).

## Inspiration

-   Zipkin lab policies: <https://github.com/zipkinlab/Policies/tree/master>

-   Bahlai lab policies: <https://github.com/BahlaiLab/Policies>

-   Tendler, B.C., Welland, M., Miller, K.L., The WIN Handbook Team, 2023.
    Why every lab needs a handbook.
    eLife 12, e88853.
    <https://doi.org/10.7554/eLife.88853>

## How to use this template

(These instructions are a WIP and will eventually link to more detailed tutorials for each step)

1.  [Get started with Quarto](https://quarto.org/docs/get-started/)
2.  Click the green "Use this template" button on this page to create a copy in your own GitHub organization (or personal account)
3.  Clone your new repository to your computer (e.g. by [creating a new RStudio project](https://docs.posit.co/ide/user/ide/guide/tools/version-control.html#creating-a-new-project-based-on-a-remote-git-or-subversion-repository))
4.  Run `quarto preview` in the terminal to get a live preview of your book
5.  Edit the `_quarto.yml` configuration file to customize it to your group (see below)
6.  Edit the `.qmd` files to customize it to your group (see below)
7.  Delete this instructions from your `README.md`
8.  Commit your changes and push to GitHub
9.  Publish to GitHub Pages (see below)

### Things to edit

-   Do a find and replace everywhere (cmd + shift + F in RStudio) for the following: "GROUP_NAME", "PI_NAME", and "PI_EMAIL".

-   Edit the `repo_url:` key in `_quarto.yml` to be the URL to *your* copy of this template on *your* GitHub organization or account

-   Edit the authors information in `_quarto.yml` (e.g. name and ORCID)

-   Potentially add, remove, or re-order chapters by editing the `chapters:` key in `_quarto.yml`

-   Red callout boxes titled "Group Edit" hold suggestions for what content to include on that page/section.
    These should be deleted once the edits happen.

-   **All text** in the `.qmd` documents is boilerplate or example text and intended to be edited to some extent to customize it for your group.

### To publish

You only have to do this once.

Run `quarto publish gh-pages` in the terminal to create `_publish.yml`.
Commit and push `_publish.yml` and from then on the book should automatically re-render when changes are pushed to the GitHub repo.
