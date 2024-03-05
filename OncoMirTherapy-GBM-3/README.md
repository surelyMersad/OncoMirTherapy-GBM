# OncoMirTherapy-GBM: Gene Set Enrichment Analysis in Brain Tumor Therapy

## Introduction
The "OncoMirTherapy-GBM" repository hosts the R Markdown analysis for gene set enrichment analysis focusing on the strategic targeting of oncogenic microRNAs (oncoMiRs) in the treatment of glioblastoma multiforme (GBM). This research contributes to understanding the complex gene network modulations by miRNAs and the potential of γ-modified peptide nucleic acids (PNAs) for precision medicine in brain tumor treatment.

### Study Background
This work is based on the investigation into bioengineered nanoparticle systems (BNPs) carrying anti-seed γ-modified peptide nucleic acids (sγPNAs) targeting multiple oncomiRs. Our dataset, obtained from GEO (accession ID: GSE217366), supports a promising approach for enhancing GBM therapy and personalizing treatment based on tumor-specific oncomiRs.

## Repository Content
- `OncoMirTherapy-GBM-3.Rmd`: An R Markdown document detailing the Non-thresholded Gene Set Enrichment Analysis (GSEA) and discussion of the results with visualization in Cytoscape.

## Prerequisites
To run the analysis, you need R and RStudio installed on your system. Essential packages include `ComplexHeatmap`, `circlize`, `magick`, `gprofiler2`, `Rcurl`, `RCy3`, among others. These can be installed using the following script:

```R
options(repos = c(CRAN = "http://cran.rstudio.com"))
packages <- c("devtools", "ComplexHeatmap", "circlize", "magick", "gprofiler2", "Rcurl", "BiocManager", "knitcitations", "limma", "edgeR", "ggplot2", "RCy3")
for (pkg in packages) {
  if (!requireNamespace(pkg, quietly = TRUE))
    install.packages(pkg)
}
BiocManager::install("RCy3")

