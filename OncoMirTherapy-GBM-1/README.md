## Introduction
This repository contains the first part of the project for "Strategic Targeting of OncomiRs in Brain Tumor Therapy: A Gene Expression Analysis Approach". In this part of the project we clean and normalize the data. 

### Article Reference
- Wang, Y., Malik, S., Suh, H., et al. "Anti-seed PNAs targeting multiple oncomiRs for brain tumor therapy". _Science Advances_ 9.6 (2023), p. eabq7459.

## Dataset
The dataset used in this project was obtained from the GEO database with the accession ID: GSE217366, as described in the referenced article.

## Installation

To replicate this analysis, ensure you have R and RStudio installed on your computer. Then, install the required packages using the following R commands:

```R
options(repos = c(CRAN = "http://cran.rstudio.com"))
packages <- c("devtools", "ComplexHeatmap", "circlize", "magick", "gprofiler2", "Rcurl", "BiocManager", "knitcitations")
for (pkg in packages) {
  if (!requireNamespace(pkg, quietly = TRUE))
    install.packages(pkg)
}
BiocManager::install("RCy3")
