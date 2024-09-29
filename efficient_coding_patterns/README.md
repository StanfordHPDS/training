# Efficient Coding Patterns in R and Python

Writing efficient code in R and Python can, at times, be counterintuitive. Patterns you've learned in other languages or other projects may actually be quite slow. We'll work on developing an intuition for speeding up code, explore techniques for understanding and improving code performance, implement parallel processing, and discuss other strategies like changing tools and using lower-level code like C or Rust.

## Materials

* [Hosted Slides](https://teaching-warehouse.netlify.app/efficient_coding_patterns/efficient_coding_patterns.html)
* [Repository of training materials](https://github.com/emptyfield-ds/efficient_coding_patterns)

## Pre-work

There is a bit of work to make sure you've done for this training. You'll want to make sure you have a local copy of the training materials as well as the dependencies you need.

### Python

Clone or otherwise download the repository. Once you've opened up the project, create a conda environment with the required packages installed for the workshop.

```python
conda create -n efficient_coding_env python=3.12 pandas polars pyarrow jupyter scalene -c conda-forge -y
conda activate efficient_coding_env
```

### R 

To download the repository, just run `usethis::use_course("emptyfield-ds/efficient_coding_patterns")`, which will download the materials and open a new RStudio session with the workshop open. Alternatively, clone or download from GitHub.

Once you have the project open, make sure you have the required packages installed.

```r
install.packages(
  c(
    "tidyverse", "data.table", "arrow", "bench", "profvis", 
    "future", "future.apply", "furrr", "ggbeeswarm"
  )
)
```
