# Organ Microenvironments Drive Divergent T Cell Evolution in Acute GVHD (STM 2024) Code Repo

This repository contains code and analysis to replicate the findings of Ingersoll and Bermea et al

Location of primary files can be found on the Gene Expression Omnibus database.

## Source Code

### Notebook 01
* Preparation of filtered, T-cell enriched annData object used for all downstream analysis
* Training of variational autoencoder model using scVI to generate clusters for downstream analysis

### Notebook 02
* Figure 4E: Pseudobulk differential expression lung and liver T cells

### Notebook 03
* Figure 5A, 5B, S5A, S5C: Defining clonotype "shared" and "unique" status and dividing clonotypes by degrees of expansion

### Notebook 04
* Figure 5C: Agglomerative hierarchical clustering of shared clonotypes with at least 5 clones in both organs
* Figure 5D: Euclidean distance calculation using latent space between shared clonotypes with at least 5 clones in both organs

### Notebook 05
* Figure 5E: Calculation of Jaccard similarity coefficients for cluster distributions between shared clonotypes 

### Notebook 06
* Figure 5L: Pearson correlation coefficients for cluster distribution between shared clonotypes based on degree of clonal expansion
* Figure S5B: Pearson correlation cofficients for cluster distribution between unique clonotypes based on degree of clonal expansion

### Notebook 07
* Figure S4: AUCell score generation for tissue resident memory T cell signatures

### Notebook 08
* Figures 5F-K: RNA trajectory analysis using Monocle3

## Links to External Tools (please check specific notebooks for version)
* Cellranger - https://www.10xgenomics.com/support/software/cell-ranger/latest
* Cellbender -  https://cellbender.readthedocs.io/en/latest/index.html 
* scVI - https://scvi-tools.org/
* PyDESeq2 - https://pydeseq2.readthedocs.io/en/latest/# 
* decoupler - https://decoupler-py.readthedocs.io/en/latest/
* anndata - https://anndata.readthedocs.io/en/latest/
* Scanpy - https://scanpy.readthedocs.io/en/stable/
* SciPy - https://scipy.org/
* scikit-learn - https://scikit-learn.org/stable/
* Monocle3 - https://cole-trapnell-lab.github.io/monocle3/ 
