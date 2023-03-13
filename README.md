# Assignment-7
Repo for assignment 7, exploring R packages (FISH 549)

## Description and Review of DESeq2 Package

### Location

The package is available through the Bioconductor Package. You must use the [BiocManager package](https://cran.r-project.org/web/packages/BiocManager/index.html) available via CRAN to download the DESeq2 package. This package acts as a gateway to download all Bioconductor Project R packages. To install using BiocManager, you can use this code:

```{r}
if (!require("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("DESeq2")
```

### Vignettes

Bioconductor offers a very detailed [vignette](http://bioconductor.org/packages/devel/bioc/vignettes/DESeq2/inst/doc/DESeq2.html) that runs you through using DESeq2 to run a differential expression analysis on RNA-seq data. This documentation is very detailed and hyperlinked to allow you to select which steps you would like to view.

### Applications

There are a lot of really cool use cases for DESeq2. Some of the coolest I have seen recently are using DESeq2 to see how effective treatments are at changing the expression of genes in cancer cells, using DESeq2 to examine how oysters regulate gene expression under thermal stress, and using DESeq2 to evaluate the transcriptional impacts bitter crab syndrome has on crustaceans.

DESeq2 also offers many ways to visualize differential gene expression, as seen here with the use of a shiny app to bring all of the visualizations together in one place:

![image](https://user-images.githubusercontent.com/449218/111832925-b16ae280-88f1-11eb-8530-290374f9f2c2.gif)
