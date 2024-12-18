# Organ Microenvironments Drive Divergent T Cell Evolution in Acute GVHD (STM 2025) Single Cell Analysis Code Repo

* This repository contains code and analysis to replicate the single cell analysis findings of Ingersoll and Bermea et al
* Location of the primary files, including raw data, can be found on the Gene Expression Omnibus (GEO) database (GSE284173).
* We have provided access to several processed .hdf5 files as well on GEO (GSE284173). The GEO file names correspond to the following file names in this repository as follows:
  * GSE284173.hdf5 --> 01_pre_filtered_object.hdf5
  * GSE284173_1.hdf5 --> 02_final_filtered_object.hdf5
  * GSE284173_2.hdf5 --> 03_shared_clonotype_object.hdf5
* VAE models and the Trm gene signature list are located within this repository
* Please note that this source code allows for the reproduction of data that is eventually used to create the figures found in the paper. Because many of our figures were generated using the GraphPad Prism software (Version 10, https://www.graphpad.com/), the end result of these notebooks will not result in visual output. 
* Figures 5B, 5C, S3A, S3B, and S4 can be re-created from primary data using scanpy.pl.umap (https://scanpy.readthedocs.io/en/1.10.x/api/generated/scanpy.pl.umap.html). See external tools section below for more details
* Figure S3D can be re-created from primary data using scanpy.pl.dotplot (https://scanpy.readthedocs.io/en/stable/generated/scanpy.pl.dotplot.html). See external tools section below for more details

## Source Code

### Notebook 01
* Preparation of filtered, T-cell enriched annData object used for all downstream analysis
* Training of variational autoencoder model using scVI to generate clusters for downstream analysis

### Notebook 02
* Figure 5E: Pseudobulk differential expression lung and liver T cells

### Notebook 03
* Figure 6A, 6B, S5B: Defining clonotype "shared" and "unique" status and dividing clonotypes by degrees of expansion

### Notebook 04
* Figure 6C: Agglomerative hierarchical clustering of shared clonotypes with at least 5 clones in both organs
* Figure 6D: Euclidean distance calculation using latent space between shared clonotypes with at least 5 clones in both organs

### Notebook 05
* Figure 6E: Calculation of Jaccard similarity coefficients for cluster distributions between shared clonotypes 

### Notebook 06
* Figure 6L: Pearson correlation coefficients for cluster distribution between shared clonotypes based on degree of clonal expansion
* Figure S5A: Pearson correlation cofficients for cluster distribution between unique clonotypes based on degree of clonal expansion

### Notebook 07
* Figure S4: AUCell score generation for tissue resident memory T cell signatures

### Notebook 08
* Figures 6F-K: RNA trajectory analysis using Monocle3

## Links to External Tools
### Please check specific notebooks for version information
* Cellranger (v.7.0.0) - https://www.10xgenomics.com/support/software/cell-ranger/latest
* Cellbender (v0.2.0) -  https://cellbender.readthedocs.io/en/latest/index.html 
* scVI (v<0.15.0) - https://scvi-tools.org/
* PyDESeq2 (v0.4.10) - https://pydeseq2.readthedocs.io/en/latest/# 
* decoupler (v1.6.0) - https://decoupler-py.readthedocs.io/en/latest/
* anndata (see notebook for version) - https://anndata.readthedocs.io/en/latest/
* Scanpy (see notebook for version) - https://scanpy.readthedocs.io/en/stable/
* SciPy (v1.12.0) - https://scipy.org/
* scikit-learn (v1.5.1) - https://scikit-learn.org/stable/
* Monocle3 (v1.3.7) - https://cole-trapnell-lab.github.io/monocle3/
* Zellkonverter (v.1.12.1) - https://bioconductor.org/packages/release/bioc/html/zellkonverter.html
* SingleCellExperiment (v1.24.0) - https://bioconductor.org/packages/release/bioc/html/SingleCellExperiment.html
