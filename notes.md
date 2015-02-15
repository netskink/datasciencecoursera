---
title: "notes.md"
author: "John F. Davis"
date: "Saturday, February 14, 2015"
output: html_document
---

This is an R Markdown document. Markdown is a simple formatting syntax for authoring HTML, PDF, and MS Word documents. For more details on using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that includes both content as well as the output of any embedded R code chunks within the document. You can embed an R code chunk like this:

```{r}
summary(cars)
```

You can also embed plots, for example:

```{r, echo=FALSE}
plot(cars)
```

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.

# My Notes
## this is a secondary heading
### This is a tertiary heading

## This a bulleted list
* item 1
* item 2
* item 3

## An introduction to markdown is here
http://www.daringfireball.net/projects/markdown

## This how to install packages in R
a<-available.packages()
head(rownames(a),3)  ## show the names of the first few packages
install.packages("slidify")
install.packages(c("slidify","ggplot2", "devtools"))


You can also use Tools->Install Packages in RStudio

## Install packages from Bioconductor
source("http://bioconductor.org/biocLite.R")

Then next time to install a package
biocLite(c("GenomicFeatures","AnnotationDbi"))

## Load a package
After you install a package, you need to use library() to use the functions of that package
library(ggplot2)  ## No quotes

## Search functions of a packages
library(ggplot2)  ## Add the functions to top of the functions list?
search() 

## Websites for searching R programming tips
www.rseek.org

## install devtools package
http://cran.r-project.org/bin/windows/Rtools/ 
install.packages("devtools")
find_rtools()