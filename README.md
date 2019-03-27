# Cell type specific analyses

This repository contains an RMarkdown document including a "complete" version with full R code to perform to identify disease-relevant Substantia nigra cell types across 33 diseases and traits with LDSCORE

## Material

This repository contains R data object and RMarkdown documents that can be used for the analysis of the datasets. 

**R Data objects:** 

* TPM expression matrix and the SN cell types identified: `Devika_midbrain.Rdata`
* t-statistic results generated for each gene for different cell type in the SN: `Mid_t_test.Rdata`

**Rmd file:**

There is RMarkdown document including a "complete" version with full R code. 

* Data analysis: `LDSCORE_Analysis_SN.Rmd`

## LSCORE

You will need to download here and install LDSCORE software here: https://github.com/bulik/ldsc

## R packages

You will need to have the following R packages installed: `biomaRt`,`reshape2`. We will use the development versions of the Bioconductor packages.

```{r}
install.packages(c("reshape2"))
## try http:// if https:// URLs are not supported
if (!requireNamespace("BiocManager", quietly = TRUE))
install.packages("BiocManager")
BiocManager::install("biomaRt")
```

## Useful Resources

* `LDSCORE publication` : Heritability enrichment of specifically expressed genes identifies disease-relevant tissues and cell types
https://www.nature.com/articles/s41588-018-0081-4


