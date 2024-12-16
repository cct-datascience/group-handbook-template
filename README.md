# Lab Group Handbook Template

<!-- badges: start -->

[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.14502303.svg)](https://doi.org/10.5281/zenodo.14502303)

<!-- badges: end -->

This repo provides a template for a wiki-like lab group handbook built as a [Quarto book](https://quarto.org/docs/books/).
A lab group handbook is a document that conveys a lab's ethos, policies, and procedures to group members ([Tendler et al., 2023](https://doi.org/10.7554/eLife.88853)).
Some of the content is University of Arizona specific (e.g. links in the code of conduct), but it is intended for use by anyone with any kind of lab group (or other group) to adopt!

## Features

-   Write content as Quarto documents (.qmd), markdown (.md), RMarkdown (.Rmd), or even jupyter notebooks (.ipynb)
-   Built-in search bar
-   Each page has a link to create a GitHub pull request to make an edit or to open an issue suggesting edits
-   Automatic deployment to GitHub pages with GitHub actions
-   A "research best practices" page with our group's suggestions for creating reproducible research compendia
-   A Code of Conduct with links to University of Arizona policies and reporting forms
-   All the features of [Quarto](https://quarto.org/)!

## Tutorial

I ran a workshop on using this template at University of Arizona.
You can watch the [video](https://img.youtube.com/vi/ad-1P11O5a4) or check out the [slides](https://cct-datascience.quarto.pub/creating-a-lab-group-handbook-with-quarto/#/title-slide).

[![Title slide reading "Creating a Lab Group Handbook with Quarto / Eric R. Scott / 2024-08-28](https://img.youtube.com/vi/ad-1P11O5a4/0.jpg)](https://youtu.be/ad-1P11O5a4?si=lQh9TwT6ccMDfT6t)

## Inspiration

-   Zipkin lab policies: <https://github.com/zipkinlab/Policies/tree/master>

-   Bahlai lab policies: <https://github.com/BahlaiLab/Policies>

-   Tendler, B.C., Welland, M., Miller, K.L., The WIN Handbook Team, 2023.
    Why every lab needs a handbook.
    eLife 12, e88853.
    <https://doi.org/10.7554/eLife.88853>

There is a [growing list of open lab group handbooks](https://github.com/cct-datascience/open-lab-handbooks) that you can get inspiration from (with proper credit of course!)

## How to use this template

1.  [Use this template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template)—click the green "Use this template" button on this page to create a copy in your own GitHub organization (or personal account)
2.  Clone your new repository to your computer (e.g. by [creating a new RStudio project](https://docs.posit.co/ide/user/ide/guide/tools/version-control.html#creating-a-new-project-based-on-a-remote-git-or-subversion-repository))
3.  [Preview your book](https://quarto.org/docs/books/#book-preview) by running `quarto preview` in the terminal
4.  Edit the `_quarto.yml` configuration file to customize it to your group (see below)
5.  Edit the `.qmd` files to customize it to your group (see below)
6.  Delete these instructions from your `README.md` (and please credit this template!)
7.  Commit your changes and push to GitHub
8.  Publish to GitHub Pages by running `quarto publish gh-pages` (see below)

See [Get started with Quarto](https://quarto.org/docs/get-started/) and the [Quarto book documentation](https://quarto.org/docs/books/) for more on customizing this template.

### Things to edit

In `README.md`

-   Edit this to be about your book, rather than about how to use the template

In `_quarto.yml`

-   `book: title:`

-   `book: repo-url:` should point to the GitHub repo of *your* copy of this template on *your* GitHub organization or account

-   `book: author:` Edit the authors information in `_quarto.yml` (e.g. name and ORCID) and potentially add authors

-   Potentially add, remove, or re-order chapters by editing the `chapters:` key in `_quarto.yml`

In the various `.qmd` files

-   Do a find and replace everywhere (cmd + shift + F in RStudio) for the following: "GROUP_NAME", "PI_NAME", and "PI_EMAIL".

-   Red callout boxes titled "Group Edit" hold suggestions for what content to include on that page/section.
    These should be deleted once the edits happen.

-   **All text** in the `.qmd` documents is boilerplate or example text and intended to be edited to some extent to customize it for your group.

`CITATION.cff`

-   Remove this file or edit to refer to your book rather than this template repo.

-   More on cff files: <https://citation-file-format.github.io/>

-   On adding citation metadata to your book: <https://quarto.org/docs/reference/metadata/citation.html>

### To preview

In the terminal run `quarto preview` and it should open a live preview of your book in a browser window.
When you make changes and save them, this preview will update.

### To publish

You only have to do this once.

In the terminal, stop the `quarto preview` process if it is running, run `quarto render` and then `quarto publish gh-pages`.
When this is successful it should open up your book in your web browser.
After this, the GitHub action included in `.github/` should automatically re-render and deploy your book when changes are pushed to the main branch on GitHub.
