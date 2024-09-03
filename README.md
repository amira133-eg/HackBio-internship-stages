# Exploring R Packages in Cancer Research: Tools, Applications, and Innovations

# Authors (@slack): Amira Mahmoud Mohamed (amira\_mahmoud\_4463)

Packages in R are collections of functions that play important roles in handling different types of data. packages are  more than one function to do action.sach as,Gene expression profiling is a useful way to measure the activity of genes in molecular biology . because of its effectiveness. the researchers have released thousands of gene expression datasets publicly in online databases and repositories. such as Gene Expression Omnibus (GEO). To read and analyze gene expression data, the computational biology community has developed several tools and platforms including Bioconductor . an R open-source platform of software packages that can be used to analyze these data. Despite the usefulness of Bioconductor and of its packages,.it is still difficult to read gene expression data from GEO for example . and to assign gene symbols to the probesets of datasets. To alleviate this problem, we introduce here a new R software package, geneExpressionFromGEO,which provides to the users the possibility to easily download gene expression data from GEO and to easily associate gene symbols to probesets. so that , we can install R packages from Bioconductor or CRAN to make mor than one function in same time.

### How to install R packages from CRAN

### To download CRAN packages, start by searching for the desired CRAN packages on Google. Once you have identified the package you need, open RStudio and write the code to install the package. For example, to install a package, you would use the command `install.packages("package_name")`. After the package is installed, you need to call it in your R session using the `library` function. To do this, you would write `library(package_name)`. You can then see the functions available in the package.

### For example, a package downloaded from CRAN, **`ggplot2 package`,** is used to visualize relationships between different genes or between gene expression levels and other variables. It is also useful for visualizing differential expression results, where you can plot fold changes against significance levels.

### **HOW to install R Packages from Bioconductor** 

### For Bioconductor packages, start by searching on Google for the package you need. Once you have identified the package and understand its name and function, you should go to the installation process. If you do not have BiocManager installed, use the following code to install it

### `if (!require("BiocManager", quietly = TRUE))`

###     `install.packages("BiocManager")`

### Then, you can install the Bioconductor package you need. For example, to install the `GEOquery` package, you would use:

### `BiocManager::install("GEOquery)`

### After installing the package, open RStudio, paste the installation command, and run it. To load the package, use the `library` function with the package name. For instance, `library(GEOquery)` will load the `GEOquery` package. The package will contain more than one function for application



### it relates to cancer ##

### For example, the **`DESeq2` package** from Bioconductor is used for differential gene expression analysis from count data. This package provides a robust workflow for RNA-Seq data analysis, including normalization to account for differences in sequencing depth, statistical testing for differential expression, and visualization tools for results. In breast cancer research, the `DESeq2` package plays a crucial role in analyzing RNA-Seq data to understand gene expression patterns in breast cancer. Certainly, we summarize the importance of The DESeq2 package in R is for breast cancer research because it analyze RNA sequencing data to understand gene expression changes in cancer cells compared to normal cells.This can help us in discovering potential biomarkers and therapeutic targets for treatment. 

for example 2 ,The **`GEOquery` package** in R is crucial for breast cancer research because it allows scientists to access and download gene expression data from the Gene Expression Omnibus **(GEO) database**. This database contains a vast repository of publicly available gene expression datasets from various studies, including those related to breast cancer. Using `GEOquery`, researchers can easily retrieve and analyze data to explore gene expression patterns, identify biomarkers, and understand disease mechanisms.Examples of its application: `GEOquery` to obtain RNA-Seq or microarray data from GEO, which they then analyze to identify differentially expressed genes in breast cancer.

## references ##

Anders, S., et al. [Count-based differential expression analysis of RNA sequencing data using R and Bioconductor.](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?db=PubMed\&cmd=Search\&doptcmdl=Citation\&defaultField=Title+Word\&term=Count-based+differential+expression+analysis+of+RNA+sequencing+data+using+R+and+Bioconductor.&\_\_hstc=48295481.db2875411e1f9ace171c565e59acc22c.1725400450469.1725400450469.1725400450469.1&\_\_hssc=48295481.1.1725400450470&\_\_hsfp=280987615) *Nature Protocols*. 8, 1765-1786 (2013).

McDermaid, A., Monier, B., Zhao, J., Liu, B., Ma, Q. [Interpretation of differential gene expression results of RNA-seq data: review and integration.](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?db=PubMed\&cmd=Search\&doptcmdl=Citation\&defaultField=Title+Word\&term=Interpretation+of+differential+gene+expression+results+of+RNA-seq+data:+review+and+integration.&\_\_hstc=48295481.db2875411e1f9ace171c565e59acc22c.1725400450469.1725400450469.1725400450469.1&\_\_hssc=48295481.1.1725400450470&\_\_hsfp=280987615) *Briefings in Bioinformatics*. 20, 2044-2054 (2019).

Taub F, DeLeo J, Thompson EB (1983) Sequential comparative hybridizations analyzed by computerized image processing can identify and quantitate regulated RNAs. DNA 2(4):309–327

[Article](https://doi.org/10.1089%2Fdna.1983.2.309) **[CAS](https://link.springer.com/articles/cas-redirect/1%3ACAS%3A528%3ADyaL2cXmsVCktg%253D%253D) [Google Scholar](https://scholar.google.com/scholar\_lookup?\&title=Sequential%20comparative%20hybridizations%20analyzed%20by%20computerized%20image%20processing%20can%20identify%20and%20quantitate%20regulated%20RNAs\&journal=DNA\&volume=2\&issue=4\&pages=309-327\&publication\_year=1983\&author=Taub%2CF\&author=DeLeo%2CJ\&author=Thompson%2CEB)

American Cancer Society. (2022, March 1).  
Survival Rates for Breast Cancer. AmericanCancerSociety. [https://www.cancer.org/cancer/breast-cancer/understanding-a-breast-cancer-diagnosis/breast-cancer-survival-rates.html](https://www.cancer.org/cancer/breast-cancer/understanding-a-breast-cancer-diagnosis/breast-cancer-survival-rates.html)

UCLA Statistical Methods and Data Analytics. (n.d.).Logit Regression | R Data Analysis Examples.Retrieved August 22, 2022, from [https://stats.oarc.ucla.edu/r/dae/logit-regression/](https://stats.oarc.ucla.edu/r/dae/logit-regression/)

