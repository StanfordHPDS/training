# Data Validation in R and Python

We often have unspoken or unexplored expectations about our data. Data validation makes those expectations explicit and provides us a method to automatically test for them. This process is useful for verifying new data, guiding data manipulation, and checking that changes to data aren't going to cause code to fail. In this training, we'll learn the pointblank package for R and Python to validate data.

## Materials

* [Hosted Slides](https://teaching-warehouse.netlify.app/data_validation/data_validation.html)
* [Repository of training materials](https://github.com/emptyfield-ds/data_validation)

## Pre-work

There is a bit of work to make sure you've done for this training. You'll want to make sure you have a local copy of the training materials as well as the dependencies you need.

### Python

Clone or otherwise download the repository. Once you've opened up the project, create a conda environment with the required packages installed for the workshop.

```python
conda create -n data_validation_env python=3.12 pandas polars -c conda-forge -y
conda activate data_validation_env
pip install pointblank
```

### R 

To download the repository, just run `usethis::use_course("emptyfield-ds/data_validation")`, which will download the materials and open a new RStudio session with the workshop open. Alternatively, clone or download from GitHub.

Once you have the project open, make sure you have the required packages installed.

```r
install.packages(c("tidyverse", "pointblank"))
```
