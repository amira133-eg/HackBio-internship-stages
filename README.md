# Stage-0-
 Learning Track : Frontend Bioinformatics    ( How to install packages in R )
  
How to install Packages in R

Before that, we ask ourselves how we know the rise and fall in the expression of a breast tumor, and how the programming language R makes it easier for us to understand different gene expression?
First we know what is
 Packages are a group of functions that play important roles in different data types
( packages \= more than function \= make an action )
Secondly, packages are created from outside the r base, so they are created from a source outside   
Such as CRANA, BIOCONDUCTOR, GITHUB We have more than method to install packages  
Let's expand on it

How to install Packages in R 

 crna packages How to download them

1- Search for crna packages from Google

2- install packages by names

3- open R studio and write the code

(installpackages("package name")

4- to call the package which you installed, make function named (library)

5- wite name of package which you make library ::

6- You can see the functions in the package

example for dowenloaded package from CRNA (ggplot2) to visualize relationships between different genes or between gene expression levels and other variables and for visualizing differential expression results, where you plot fold changes against significance levels

Another way with us

how to install r packages from bioconductor

1- Search on Google for bioconductor packages

2-We can search on the package you want and known its name and function

3- go to installation then copy of

 if (\!require("BiocManager", quietly \= TRUE))

    install.packages("BiocManager")

 

BiocManager::install("GEOquery")

 

4- open R studio and past then run

5-bioconductor::install("package name")

6- The package is installed contain more than function

 

For example we can install DESeq2 package from Bioconductor for differential gene expression analysis from count data, and

The package provides a robust workflow for RNA-Seq data analysis, including normalization to account for differences in sequencing depth, statistical testing for differential expression, and visualization tools for results

In breast cancer research, the DESeq2 package plays a crucial role in analyzing RNA-Seq data to understand gene expression patterns, identify potential biomarkers, and gain insights into the underlying mechanisms of the disease. Here’s why DESeq2 is particularly important in the context of breast cancer research

 

By analyzing gene expression data from breast cancer samples, researchers can gain insights into the molecular mechanisms driving tumor development and progression. Differential expression analysis helps identify pathways and processes that are altered in breast cancer

 

 

 

