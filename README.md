# vikasinisenthil.github.io

## About
This repository contains my Quarto website and blog, including palmer penguins data analyses written in R and Python.

## What to install
Install these tools before building the site:
- Quarto 1.10.18
- uv 0.12.7
- R version 4.6.1
- Python 3.14.7

`uv.lock` lists the Python packages needed for this site. 

`renv.lock` lists the R packages needed for this site.

## Build the site
Run these commands in Git Bash:
```bash
git clone git@github.com:vikasinisenthil/vikasinisenthil.github.io.git
cd vikasinisenthil.github.io
uv sync
Rscript -e 'renv::restore()'
uv run quarto render
```

## View the site locally
The built site is in `docs/`

Open `docs/index.html/` in a browser to see the site. 

To open the two posts using `docs/posts/penguins-python/index.html` and `docs/posts/penguins-r/index.html`


## Data
Both posts use the Palmer penguins dataset from the `palmerpenguins` package. The data comes with the packages. You do need internet access to install the Python and R packages.