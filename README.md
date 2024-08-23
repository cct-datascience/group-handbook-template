# group-handbook-template

<!-- badges: start -->

[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)

<!-- badges: end -->

This is a work-in-progress template for a lab group handbook much like the one described by [Tendler et al., 2023](https://doi.org/10.7554/eLife.88853).
Some of the content is University of Arizona specific (e.g. links in the code of conduct), but it is intended for use by anyone with any kind of lab group (or other group) to adopt!

## Features

-   Write content as Quarto documents (.qmd), markdown (.md), RMarkdown (.Rmd), or even jupyter notebooks (.ipynb)
-   Built-in search bar
-   Each page has a link to create a GitHub pull request to make an edit or to open an issue suggesting edits
-   Automatic deployment to GitHub pages with GitHub actions
-   A "research best practices" page with our group's suggestions for creating reproducible research compendia
-   A Code of Conduct with links to University of Arizona policies and reporting forms
-   All the features of [Quarto](https://quarto.org/)!

## Inspiration

-   Zipkin lab policies: <https://github.com/zipkinlab/Policies/tree/master>

-   Bahlai lab policies: <https://github.com/BahlaiLab/Policies>

-   Tendler, B.C., Welland, M., Miller, K.L., The WIN Handbook Team, 2023.
    Why every lab needs a handbook.
    eLife 12, e88853.
    <https://doi.org/10.7554/eLife.88853>

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

-   Do a find and replace everywhere (cmd + shift + F in RStudio) for the following: "GROUP_NAME", "PI_NAME", and "PI_EMAIL".

-   Edit the `repo_url:` key in `_quarto.yml` to be the URL to *your* copy of this template on *your* GitHub organization or account

-   Edit the authors information in `_quarto.yml` (e.g. name and ORCID)

-   Potentially add, remove, or re-order chapters by editing the `chapters:` key in `_quarto.yml`

-   Red callout boxes titled "Group Edit" hold suggestions for what content to include on that page/section.
    These should be deleted once the edits happen.

-   **All text** in the `.qmd` documents is boilerplate or example text and intended to be edited to some extent to customize it for your group.

### To preview

In the terminal run `quarto preview` and it should open a live preview of your book in a browser window. 
When you make changes and save them, this preview will update.

### To publish

You only have to do this once.

In the terminal, stop the `quarto preview` process if it is running, run `quarto render` and then `quarto publish gh-pages`. 
When this is successful it should open up your book in your web browser.
After this, the GitHub action included in `.github/` should automatically re-render and deploy your book when changes are pushed to the main branch on GitHub.
