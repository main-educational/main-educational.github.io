# [main-educational.github.io](https://main-educational.github.io)

This is the website of the educational workshop of the Montreal Artificial Intelligence and Neuroscience (MAIN) conference.
The website is built with the [jupyter book](https://jupyterbook.org/) project, and deployed using github.

### Build the book locally
- Clone this repository
- Run `pip install jupyter-book` (recommended in a virtual environment).
- For a fresh build, remove the content of `content/_build/`
- Run `jb build content/`

A static version of the book will be generated on `content/_build/html/`.

### Hosting the book

The html version of the book is hosted on the `gh-pages` branch of this repo. Navigate to your local build and run,
- `ghp-import -n -p -f content/_build/html`

This will automatically push your build to the `gh-pages` branch. More information on this hosting process can be found [here](https://jupyterbook.org/publish/gh-pages.html#manually-host-your-book-with-github-pages).
