# [main-educational.github.io](https://main-educational.github.io)

This is the website of the educational workshop of the Montreal Artificial Intelligence and Neuroscience (MAIN) conference.
The website is built with the [jupyter book](https://jupyterbook.org/) project, and deployed using github.

### Build the book locally
- Clone this repository
- Run `pip install jupyter-book` (recommended in a virtual environment).
- For a fresh build, remove the content of `content/_build/`
- Run `jb build content/`

A static version of the book will be generated on `content/_build/html/`.

### Publishing the book
A [github action](https://github.com/main-educational/main-educational.github.io/blob/main/.github/workflows/deploy-book.yml) has been setup to automatically re-build and publish the book every time a change is made to the content of the `main` branch.
