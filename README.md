# Integrating metabolic and clinical/demographic data: a simple and intuitive platform.

**IntMC** (**Int**egration of **M**etabolomics with **C**linical Data), an application capable of exploring, from a simple, dynamic and user-friendly perspective, changes in the associations between the metabolic profile, obtained by mass spectrometry (MS) or nuclear magnetic resonance (NMR), with clinical/demographic characteristics of the analyzed samples. Rapid assessment of changes in these associations has the potential to identify insights that support either the formulation of new hypotheses or direction of research targets. Emphasizing that to find them, the application uses machine learning methods.

The workflow involves the following steps: A) Load Data: entry of tables with metabolic data and clinical/demographic characteristics of the samples; B) Variable Selection; selection of the spectrum band and the clinical/demographic variable whose influence on the metabolome is to be explored; C) Analysis: visualization of the clusters obtained with the machine learning methods PCA, PLS-DA, and HCA; D) New groups: construction of data subsets if interesting.

An example of the data structure is provided in the application and can also be used to test its use. More details can be found in the article (_article address_) and the supplementary material (_address of supplementary material_).

IntMC is built on the R language (v3.6.3), with an RShiny web interface that allows you to transform complex analytics pipelines into interactive and user-friendly web applications, making them accessible to non-computing experts.

With IntMC you can work online by accessing [HERE](https://szua92-junier-marrero0guti0rrez.shinyapps.io/IntMC/) or downloading it to run locally. For the latter, you can proceed as follows (in R)


``` 
## FROM Terminal

# "~"" is the path from where you saved the file.zip
setwd("~")

# Download IntMC-master
download.file(url= paste("https://github.com/juniermarreroguti/",
                          "IntMC/archive/refs/heads/master.zip", sep=""),
              destfile ="IntMC-master.zip")

# Unzip
unzip("IntMC-master.zip")

# Rename
file.rename("IntMC-master", "IntMC")

# open RStudio into IntMC file and rub IntMC.Rmd

```


