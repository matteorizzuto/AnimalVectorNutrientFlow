# Animal-Vectored Nutrient Flow in Meta-ecosystems

This repository contains the code to replicate the numerical analyses of the model presented in Rizzuto et al. (2024) _Animal-vectored nutrient flow along different resource gradients influences the nature of local and meta-ecosystem functioning_, Ecological Modelling.

This repository contains three folders, *Code*, *Data*, and *Results*. The *Code* folder contains the following items:

  * ModelAnalysis.nb, the Wolfram Mathematica notebook we used to find the equilibria of the model, evaluate the Jacobian matrix to be used in teh local stability analysis, and calculate mathematical expresions for ecosystem functions of interest, which are used in the SupportingCode.Rmd R notebook in this folder (also available as .pdf and .txt)

  * SupportingCode.Rmd, the R markdown notebook containing the code to replicate the numerical analyses of the model and produce the figures in the manuscript and appendices. It uses relative paths to load data and save results in deticated folders. A compiled, easier to read version of this file is provided as "SupportingCode.html" in this same folder.

  * SupportingCode.bib, a bibtex file containing the references cited in the R markdown notebook.

The *Data* folder contains the following two items:

  * DATA1.csv and DATA2.csv, two datasets used in SupportingCode.Rmd, randomly generated in R using function lhs() from package lhs. Names are consistent with those using the the R notebook. Variables (i.e., columns) do not have names and are referred throughout the R notebook by their relative position, using standard R notation

The *Results* folder contains no items, as it is used to store the textual and graphic items produced by running the SupportingCode.Rmd file in *Code*.

**Additional information on reproducing our analyses**

Information on the versions of R and of the packages used is provided in the html and Rmd files.

To reproduce our model analyses, please run all code chunks or knit the SupportingCode.Rmd file. Please note that any change to the structure of the folder needs to be reflected in an update to the relative paths used in this notebook. A simple search for “../“ should be sufficient to find all instances in which relative paths are used, to update them as needed.

The code presented in ModelAnalysis.nb can be used in Wolfram Mathematica to find the model’s equilibria and evaluated the Jacobian of the single equilibrium that has biological meaning, respectively. Alternative .pdf and .txt versions of this notebook can be perused, if Wolfram Mathematica is not available.
