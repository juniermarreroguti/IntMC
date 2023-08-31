# Integrating metabolic and clinical/demographic data: a simple and intuitive platform.

<div class=text-justify>

&nbsp;&nbsp;&nbsp;
**IntMC** (**Int**egration of **M**etabolomics with **C**linical Data) is a simple, dynamic and user-friendly application capable of exploring changes in the associations between the metabolic profile obtained by mass spectrometry (MS) or nuclear magnetic resonance (NMR), and the clinical/demographic characteristics of the samples. These changes are evaluated based on machine learning methods (_Principal Component Analysis (PCA)_, _Partial Least Squares - Discriminant Analysis (PLS-DA)_, and _Hierarchical Clustering Analysis (HCA)_), and its rapid assessment  has the potential to identify insights, and therefore, support brainstorming, new hypothesis formulation and direct research targets.

&nbsp;&nbsp;&nbsp;
The workflow involves the following steps: 

<input type="checkbox" unchecked> **A.** Load Data - entry of tables with (1) _metabolic data_ and  (2) _clinical/demographic characteristics_ of the samples; </input> 
	
<input type="checkbox" unchecked> **B.** Variable Selection -  selection of the _spectrum band_ and the _clinical/demographic variable_ whose influence on the metabolome is to be explored; </input> 
	
<input type="checkbox" unchecked> **C.** Analysis: visualization of the clusters obtained by the machine learning methods available; </input> 
	
<input type="checkbox" unchecked> **D.** New groups creation - tool to build data subsets from user's inputed table, if interesting. </input> 

&nbsp;&nbsp;&nbsp;
An example of the data structure is provided in the application and can also be used to test its use. More details can be found in the article (_article address_) and the supplementary material (_address of supplementary material_).

&nbsp;&nbsp;&nbsp;
**IntMC** is built on the R language (v3.6.3), with an RShiny web interface that allows you to transform complex analytics pipelines into interactive and user-friendly web applications, making them accessible to non-computing experts.

&nbsp;&nbsp;&nbsp;
With IntMC you can work online by accessing [HERE](https://szua92-junier-marrero0guti0rrez.shinyapps.io/IntMC/) or downloading it to run locally. Latter, you can proceed as follows (in R).
</div>



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

# open RStudio into IntMC file and run IntMC.Rmd

```


