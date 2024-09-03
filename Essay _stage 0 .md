**How to install R Packages** 

Authors (@slack): Amira Mahmoud Mohamed (amira_mahmoud_4463)

Before delving into the topic, we should ask ourselves .How can we identify the up-regulated and down-regulated gene expressions in a breast tumor?, and how the R programming language facilitates our understanding of different gene expressions

First, let’s define what packages are. Packages in R are collections of functions that play important roles in handling different types of data

 ( packages \= more than one function \= perform action) 

Secondly, packages are created outside of the R base, meaning they originate from external sources such as CRAN, Bioconductor, and GitHub. There are several methods to install these packages. Let’s explore them.



### **How to install R packages from CRAN**

### To download CRAN packages, start by searching for the desired CRAN packages on Google. Once you have identified the package you need, open RStudio and write the code to install the package. For example, to install a package, you would use the command `install.packages("package_name")`. After the package is installed, you need to call it in your R session using the `library` function. To do this, you would write `library(package_name)`. You can then see the functions available in the package.

### For example, a package downloaded from CRAN, **`ggplot2 package`,** is used to visualize relationships between different genes or between gene expression levels and other variables. It is also useful for visualizing differential expression results, where you can plot fold changes against significance levels.

### **HOW to install R Packages from Bioconductor** 

### For Bioconductor packages, start by searching on Google for the package you need. Once you have identified the package and understand its name and function, you should go to the installation process. If you do not have BiocManager installed, use the following code to install it

### `if (!require("BiocManager", quietly = TRUE))`

###     `install.packages("BiocManager")`

### Then, you can install the Bioconductor package you need. For example, to install the `GEOquery` package, you would use:

### `BiocManager::install("GEOquery)`

### After installing the package, open RStudio, paste the installation command, and run it. To load the package, use the `library` function with the package name. For instance, `library(GEOquery)` will load the `GEOquery` package. The package will contain more than one function for application




### For example, the **`DESeq2` package** from Bioconductor is used for differential gene expression analysis from count data. This package provides a robust workflow for RNA-Seq data analysis, including normalization to account for differences in sequencing depth, statistical testing for differential expression, and visualization tools for results. In breast cancer research, the `DESeq2` package plays a crucial role in analyzing RNA-Seq data to understand gene expression patterns in breast cancer. Certainly, we summarize the importance of The DESeq2 package in R is for breast cancer research because it analyze RNA sequencing data to understand gene expression changes in cancer cells compared to normal cells.This can help us in discovering potential biomarkers and therapeutic targets for treatment. 

for example 2 ,The **`GEOquery` package** in R is crucial for breast cancer research because it allows scientists to access and download gene expression data from the Gene Expression Omnibus **(GEO) database**. This database contains a vast repository of publicly available gene expression datasets from various studies, including those related to breast cancer. Using `GEOquery`, researchers can easily retrieve and analyze data to explore gene expression patterns, identify biomarkers, and understand disease mechanisms.Examples of its application: `GEOquery` to obtain RNA-Seq or microarray data from GEO, which they then analyze to identify differentially expressed genes in breast cancer.

**references**

https://typeset.io/papers/r-scripts-for-user-friendly-deseq2-rna-seq-differential-dvy5hp5zer

https://typeset.io/papers/geoquery-a-bridge-between-the-gene-expression-omnibus-geo-3ouivdf51q


https://typeset.io/papers/ggplantmap-an-open-source-r-package-for-the-creation-of-33is7as4xm


**Case Study**: [GEO Data: GSE18864 \- Breast Cancer RNA-Seq Data](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE18864)

**DOWNLOAD DESeq2 package**:                  [https://www.bioconductor.org/packages/release/bioc/html/DESeq2.html](https://www.bioconductor.org/packages/release/bioc/html/DESeq2.html) 

**Download  `GEOquery` package** : [https://www.bioconductor.org/packages/release/bioc/html/GEOquery.html](https://www.bioconductor.org/packages/release/bioc/html/GEOquery.html)

