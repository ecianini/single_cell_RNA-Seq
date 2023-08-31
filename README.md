# Single cell RNA-Seq analysis
Project for the Transcriptomic course of "Bioinformatics for Computational Genomics" MSc. 

The vignette can be visualized [here](http://htmlpreview.github.io/?https://github.com/ecianini/single_cell_RNA-Seq/blob/main/singlecell_project.html).

## Aim 
In this work a single-cell RNA-Seq analysis was done for finding and characterizing liver cell subtypes. 

For a better comprehension and interpretation of the analysis results, the article [*“Single cell RNA sequencing of human liver reveals distinct intrahepatic macrophage populations”*](https://www.nature.com/articles/s41467-018-06318-7) was used as reference.

## Outline
A dataset of human parenchymal and non-parenchymal liver cells has been examined and downloaded from [PanglaoDB](https://panglaodb.se/view_data.php?sra=SRA716608&srs=SRS3391632).

Most of the steps of the analysis follow the workflow of the [Seurat vignette](https://satijalab.org/seurat/articles/pbmc3k_tutorial.html) using the Seurat package available on R. 

The project begins with loading scRNA-seq data into a Seurat object, followed by quality control steps to identify and filter out low-quality cells and genes.

Normalization methods like "LogNormalize" are employed to mitigate technical biases. Feature selection and dimensionality reduction techniques such as principal component analysis (PCA) are used to visualize the data in lower dimensions.

Clustering algorithms like Louvain and hierarchical clustering help group similar cells into clusters, which can correspond to distinct cell types, and methods to identify marker genes that define each cluster and perform differential expression analysis between clusters are used to identify genes with significant expression differences.

Visualization techniques including feature plots, UMAP plots, and cluster-specific gene expression heatmaps are used for the identification of the cell subtypes.


## References
MacParland, S.A., Liu, J.C., Ma, XZ. et al. Single cell RNA sequencing of human liver reveals distinct intrahepatic macrophage populations. Nat Commun 9, 4383 (2018)

Oscar Franzén, Li-Ming Gan, Johan L M Björkegren, PanglaoDB: a web server for exploration of mouse and human single-cell RNA sequencing data, Database, Volume 2019, 2019, baz046, https://doi.org/10.1093/database/baz046

Satija R, Farrell JA, Gennert D, Schier AF, Regev A (2015). “Spatial reconstruction of single-cell gene expression data.” Nature Biotechnology, 33, 495-502. doi:10.1038/nbt.3192, https://doi.org/10.1038/nbt.3192.



