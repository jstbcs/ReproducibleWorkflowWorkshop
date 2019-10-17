# Git and Rmarkdown: Two Useful Tools for a Fully Reproducible Workflow

This repository contains materials and slides for a workshop organized by the Open Science Community Amsterdam. It is meant as a short (two hour) teaser for different tools that can be used for a fully reproducible workflow in science. 

Licence: cc by-sa-nc 4.0

Author: Julia Haaf

## Abstract

In the debate around the reproducibility crisis, most attention is paid to instances when researchers either trick themselves or others. Recently, however, some of the discussion has also shifted to scientific and reporting mistakes sneaking into the literature without anyone noticing. Whether these are mistakes in reporting statistics (Nuijten et al., 2016) or mistakes in the data collection process (Rouder et al., 2019), they prevent computational and empirical reproducibility of results in the literature. Rouder and colleagues (2019) proposed standardization and computer automation to minimize mistakes in the literature. In this workshop I will give an introduction to two tools we used for automation in the Perception and Cognition Lab at the University of Missouri. Git is a version control system that can be used to publish data or to collaboratively work on data analysis and writing. R Markdown is a file format for making dynamic and fully reproducible documents with R where the analysis code is embedded in the text. Both tools have gained a lot of popularity in the social science workflow and form one route to a fully reproducible workflow of empirical research.

## Time and Location

October 23, at 15:00 – 17:00. Roeterseiland Campus (building G, room G S.02). 

## How to Prepare

### Install git

1. Follow the instructions here: [https://git-scm.com/book/en/v2/Getting-Started-Installing-Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).
2. Make sure to sign up with github ([github.com](github.com)), we will use it as host for our repositories.
3. We will use `RStudio` as user interface for `git`. An alternative is, for example, the github desktop GUI ([link](https://desktop.github.com/)).

### Install R and RStudio

**Windows**

Follow the instructions here: [https://www.reed.edu/data-at-reed/software/R/r_studio_pc.html](https://www.reed.edu/data-at-reed/software/R/r_studio_pc.html). 

*Note 1:* The versions in the instructions are out of date. Always install the latest release.

*Note 2:* The instructions also ask to install `MiKTeX` which we'll need as well. If you already use latex you can ignore this step because you most likely already have it installed. Make sure to try Steps 7 and 8 in this case. 

**Mac**

Follow the instructions here: [https://medium.com/@GalarnykMichael/install-r-and-rstudio-on-mac-e911606ce4f4](https://medium.com/@GalarnykMichael/install-r-and-rstudio-on-mac-e911606ce4f4).

*Note:* The versions in the instructions are out of date. Always install the latest release.

**Ubuntu 19.04/18.04/16.04**

- For `R`: Open the terminal (Ctrl+Alt+t) and type

```
sudo apt update
sudo apt install r-base
```

- For `RStudio`: Go to [https://rstudio.com/products/rstudio/download/#download](https://rstudio.com/products/rstudio/download/#download) and choose the installer for your system; follow the instructions.

### Install some R packages

- Open an `R` console, for example by opening `RStudio`.
- Type into the R console:

```
install.packages("rmarkdown")
install.packages("knitr")
install.packages("devtools")
devtools::install_github("crsh/papaja", ref = "devel")
```



