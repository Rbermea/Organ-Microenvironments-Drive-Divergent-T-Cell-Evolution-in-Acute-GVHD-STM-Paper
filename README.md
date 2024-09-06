# Organ Microenvironments Drive Divergent T Cell Evolution in Acute GVHD (STM 2024) Code Repo

This repository contains code and analysis to replicate the findings of Ingersoll and Bermea et al
## Contents

This repo shows how the following computational methods were implemented:

* Removal of ambient RNA from Cellranger multi output using Cellbender
* Preparation of filtered, T-cell enriched annData object used for all downstream analysis
* Training of variational autoencoder model using scVI to generate clusters
* Figure 4E-F: Pseudobulk differential expression lung and liver T cells
* Figure 5A: Division of clonotypes by degrees of expansion
* Figure 5C: Agglomerative hierarchical clustering of shared clonotypes with at least 5 clones in both organs
* Figure 5D: Euclidean distance calculation using latent space between shared clonotypes with at least 5 clones in both organs
* Figure 5E: Calculation of Jaccard similarity coefficients for cluster distributions between shared clonotypes 
* Figure 5F-K: RNA trajectory analysis using Monocle3
* Figure 5L: Pearson correlation coefficients for cluster distribution between shared clonotypes based on degree of clonal expansion
* Figure S4: AUCell score generation for tissue resident memory T cell signatures
* Figure S5: Pearson correlation cofficients for cluster distribution between unique clonotypes based on degree of clonal expansion

## Links to External Tools
* Cellranger
* Cellbender
* scVI
* PyDESeq2
* Monocle3
