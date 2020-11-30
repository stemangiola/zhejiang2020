<!-- badges: start -->
[![DOI](https://zenodo.org/badge/306182457.svg)](https://zenodo.org/badge/latestdoi/306182457)
[![.github/workflows/basic_checks.yaml](https://github.com/stemangiola/zhejiang2020_tidytranscriptomics/workflows/.github/workflows/basic_checks.yaml/badge.svg)](https://github.com/stemangiola/zhejiang2020_tidytranscriptomics/actions) [![Docker](https://github.com/Bioconductor/BioC2020/raw/master/docs/images/docker_icon.png)](https://hub.docker.com/repository/docker/stemangiola/zhejiang2020_tidytranscriptomics) 	
<!-- badges: end -->

# Introduction to bulk and single-cell RNA sequencing analyses
<p float="left">
<img height="100" alt="zhejiang2020" src="man/figures/zhejiang_logo.png"/> 
</p>

## Instructor names and contact information

* Xueyi Dong <dong.x at wehi.edu.au>
* Luyi Tian <tian.l at wehi.edu.au>
* Hongke Peng <peng.h at wehi.edu.au>
* Stefano Mangiola <mangiola.s at wehi.edu.au>

## Syllabus

Material [web page](https://stemangiola.github.io/zhejiang2020/).

This material was created for the [Zhejiang 2020 workshop](https://zhejiang2020.bioconductor.org/) workshop but it can also be used for self-learning.

More details on the workshop are below.

## Workshop package installation 

This is necessary in order to reproduce the code shown in the workshop. The workshop is designed for R `4.0` and can be installed using one of the two ways below.

### Via Docker image

If you're familiar with [Docker](https://docs.docker.com/get-docker/) you could use the Docker image which has all the software pre-configured to the correct versions.

```
docker run -e PASSWORD=abc -p 8787:8787 stemangiola/zhejiang2020:zhejiang2020
```

Once running, navigate to <http://localhost:8787/> and then login with
`Username:rstudio` and `Password:abc`.

You should see the Rmarkdown file with all the workshop code which you can run.

### Via GitHub

Alternatively, you could install the workshop using the commands below in R `4.0`.

```
# Install dependency manually
(to be completed)

# Install workshop package
remotes::install_github("stemangiola/zhejiang2020", build_vignettes = TRUE)

# To view vignettes
library(zhejiang2020)
browseVignettes("zhejiang2020")
```

## Workshop Description

This workshop will present how to perform analysis of bulk and single-cell RNA sequencing count data following base R paradigm. Example of the use of tidy paradigm is given at the end of each section.

The bulk analyses were based on the Bioconductor workflow package [RNAseq123](https://www.bioconductor.org/packages/devel/workflows/vignettes/RNAseq123/inst/doc/limmaWorkflow.html) and the workshop for tidy transcriptomics [BioC Asia 2020](https://stemangiola.github.io/biocasia2020_tidytranscriptomics/)

### Pre-requisites

* Basic knowledge of RStudio
* Familiarity with R base and tidyverse syntax

Recommended Background Reading
[Introduction to R for Biologists](https://melbournebioinformatics.github.io/r-intro-biologists/intro_r_biologists.html)

### Workshop Participation

The workshop format is 2 days, 2 hours sessions each day consisting of hands-on demos with Q&A.

### _R_ / _Bioconductor_ packages used

* dittoSeq
* dplyr
* edgeR
* ggplot2
* ggrepel
* Glimma
* gplots
* igraph
* limma
* Mus.musculus
* purrr
* R.utils
* RColorBrewer
* readr
* RNAseq123
* scater
* scran
* SingleCellExperiment
* SingleR
* stats
* stringr
* SummarizedExperiment
* tibble
* tidybulk
* tidyr
* tidySingleCellExperiment
* utils

### Time outline

First day

| Activity                                 | Time    |
|------------------------------------------|---------|
| Bulk RNA sequencing analyses             | 1h 20m  |
| Questions                                | 20m     |
| Break                                    | 30m     |
| Tidy bulk RNA sequencing analyses        | 30m     |
| Questions                                | 20m     |

Second day

| Activity                                 | Time    |
|------------------------------------------|---------|
| Single-cell RNA sequencing analyses      | 1h 20m  |
| Questions                                | 20m     |
| Break                                    | 30m     |
| Tidy single-cell RNA sequencing analyses | 30m     |
| Questions                                | 20m     |

### Workshop goals and objectives

In exploring and analysing RNA sequencing count data, there are a number of key concepts, such as filtering, scaling, dimensionality reduction, hypothesis testing, clustering and visualisation, that need to be understood. 

#### Learning goals

* To understand the key concepts and steps of RNA sequencing count data analysis
* Apply the concepts to publicly available data
* Create plots that summarise the information content of the data and analysis results
* To approach critical thinking
