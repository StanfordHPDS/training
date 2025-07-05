# Quarto

[Quarto](https://quarto.org/) is a framework for scientific publishing that allows you to weave narrative text together with code and code results. It's also an important tool for reproducibilty: not only is it easier to regenerate documents dynamically using Quarto, it also encourages best practices in making sure your code *can* regenerate them.

This training comes in R and Python flavors. Both flavors have cloud versions where you can participate without needing to install anything on your local computer.

## Hosted Slides

* [Slides (R)](https://teaching-warehouse.netlify.app/quarto_basics/quarto_basics.html)
* [Slides (Python)](https://teaching-warehouse.netlify.app/py_quarto_basics/py_quarto_basics.html)

## Installing Quarto

Install the [latest version of Quarto](https://quarto.org/docs/get-started/) from the website.

If you're using RStudio, it probably has a version of Quarto included, but there's no harm in installing it again. You might want to to update it, as they are actively improving it.

## R

### Learn on your computer

We'll use RStudio for the R-flavored tutorial. You can learn more about the VS Code Quarto workflow from the slides in the Python flavors.

To install the materials we need for the workshop, install the rrr.workshop package:

```r
options(repos = c(
  emptyfieldds = "https://emptyfield-ds.r-universe.dev",
  CRAN = "https://cran.rstudio.com/"
))

install.packages("rrr.workshop")
```

`rrr.workshop::use_module()` will install the materials for a given module on your computer. Then, it will open a new RStudio Project containing the files you’ll need.

```r
rrr.workshop::use_module("module_name")
```

By default, this package downloads the materials to a conspicuous place like your Desktop. You can also tell use_module() exactly where to put the materials with destdir:

```r
rrr.workshop::use_module("module_name", destdir = "a/path/on/your/computer")
```

The two modules we'll use are called `quarto_whole_game` and `quarto_basics`.

```r
rrr.workshop::use_module("quarto_whole_game")
rrr.workshop::use_module("quarto_basics")
```

### Learn on the cloud

Each module also has a cloud-hosted version on Posit Cloud. You'll need a free account. This is a good option of you want quick access without needing to install packages or downloading materials, or if you are having installation issues.

`rrr.workshop::browse_cloud("module_name")` will open the Posit Cloud project in your browser.

```r
rrr.workshop::browse_cloud("quarto_whole_game")
rrr.workshop::browse_cloud("quarto_basics")
```

## Python

### Learn on your computer

For this training, we'll use [VS Code](https://code.visualstudio.com/) with the [Quarto](https://marketplace.visualstudio.com/items?itemName=quarto.quarto) and [Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) extensions. You'll also want to make sure you have the [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python), although VS Code will likely offer to install this for you.

You can learn more about the RStudio Quarto workflow from the slides in the R flavors.

We have two modules, each of which involves the same steps for setup. You'll need [uv](docs.astral.sh/uv) to set up the local Python version and dependencies.

1. [Clone the repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) onto your local computer.
2. Run `uv sync`. This will also create a virtual environment in the `.venv/` folder.
3. In VS Code, [set the Python interpreter](https://code.visualstudio.com/docs/python/environments#_working-with-python-interpreters) to use the virtual environment in the `.venv` folder. This will sync the terminal, Jupyter, and Quarto all to use the same Python version and environment.

Here are the repositories:

1. [Quarto: The Whole Game](https://github.com/emptyfield-ds/py_quarto_whole_game)
2. [Quarto: The Basics](https://github.com/emptyfield-ds/py_quarto_basics)

### Learn on the cloud

Both repositories also have infrastucture files to automatically set up a [GitHub Codespace](https://docs.github.com/en/codespaces/getting-started/quickstart). Follow the instructions in the documentation to launch a Codespace from the repository.

When the Codespace is ready, it will open VS Code in your browser. Then, it will automatically install the necessary extensions and packages. This can take a little bit to take effect, so open it sooner than later.
