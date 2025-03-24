# Pipelines in R and Python

Pipeline frameworks are ways of managing our code execution. They keep track of the relationships between code, cache results, and only run what needs to be run. They also make it easy to run a project from scratch with a single command.

For R, we'll be learning targets. For Python, we'll be learning Make.

## Materials: R (targets)

* [Hosted Slides](https://teaching-warehouse.netlify.app/targets_basics/targets_basics.html)
* [Repository of training materials: targets basics](https://github.com/emptyfield-ds/targets_basics)
* [Repository of training materials: targets whole game](https://github.com/emptyfield-ds/targets_whole_game)

## Materials: Python (make)

* [Hosted Slides](https://teaching-warehouse.netlify.app/make_basics/make_basics.html)
* [Repository of training materials: Make basics](https://github.com/emptyfield-ds/make_basics)
* [Repository of training materials: Make whole game](https://github.com/emptyfield-ds/make_whole_game)

## Pre-work

There is a bit of work to make sure you've done for this training. You'll want to make sure you have a local copy of the training materials as well as the dependencies you need.

### Python

You'll need [uv](https://docs.astral.sh/uv/getting-started/installation/) installed for this workshop.

Clone or otherwise download the repositories. Once you've opened up the projects, sync the virtual environment in each with uv:

```python
uv sync
```

### R 

To download the repository, just run `usethis::use_course("emptyfield-ds/targets_basics")`, which will download the materials and open a new RStudio session with the workshop open. Alternatively, clone or download from GitHub.

Do the same for `usethis::use_course("emptyfield-ds/targets_whole_game")`

Once you have the project open, make sure you have the required packages installed.

```r
install.packages(c("tidyverse", "targets", "tarchetypes", "gapminder", "cowplot", "maps", "scales", "scico", "sf"))
```
