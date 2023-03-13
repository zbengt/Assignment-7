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

### Review

The primary use of this package is to estimate variance-mean dependence in count data from high-throughput sequencing assays and test for differential expression based on a model using the negative binomial distribution. Essentially, this package allows you to examine how different treatments, conditions, or groups differ in gene expression. This package is an excellent one stop shop for examining differential expression and displaying results in a variety of ways. I especially like the documentation available that easily allows you to create volcano plots and heat maps as well as complete a PCA. However, I wish that this package included a means to import data in the necessary format to run it through the model. The package itself is pretty easy to learn how to use, thanks to documentation, but getting data into the correct format for use can be a tricky sticking point. I would recommend this package to anyone looking for a comprehensive means to analyze RNA-seq data. I myself am currently using this package to examine long non-coding RNA expression differences in oysters exposed to varying ocean acidification conditions. There are other options for differential expression analysis, but DESeq2 is tried and true, while also remaining current with updates to analyze any type of high throughput sequencing data—keeping pace with constantly evolving next generation sequencing data outputs. 