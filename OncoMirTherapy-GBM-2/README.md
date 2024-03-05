# Strategic Targeting of OncomiRs in Brain Tumor Therapy: A Gene Expression Analysis Approach

## Introduction
This repository contains the R code and data for the project "Strategic Targeting of OncomiRs in Brain Tumor Therapy: A Gene Expression Analysis Approach" by Mersad Abbasi. This part of the project focuses on Differential Expression Analysis and Visualization.

## Dataset
The dataset used in this analysis, `GSE217366`, is obtained from GEO and is related to the study : Anti-seed PNAs targeting multiple oncomiRs for brain tumor therapy.

## Setup
To run the analysis, you need to have R installed on your system. After installing R, you need to install the following packages if you haven't already:

```R
# Install required packages
if (!requireNamespace("devtools", quietly = TRUE)) install.packages("devtools")
if (!requireNamespace("ComplexHeatmap", quietly = TRUE)) install.packages("ComplexHeatmap")
if (!requireNamespace("circlize", quietly = TRUE)) install.packages("circlize")
if (!requireNamespace("magick", quietly = TRUE)) install.packages("magick")
if (!requireNamespace("gprofiler2", quietly = TRUE)) install.packages("gprofiler2")

# Load the packages
library(ComplexHeatmap)
library(circlize)
library(knitr)
library(limma)
library(edgeR)
library(ggplot2)
library(magick)
library(gprofiler2)
