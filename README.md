# trio-hippocampus-rnaseq
Differential expression and pathway analysis of synaptosomal RNA-seq data

This script processes bulk RNA-seq count data from mouse hippocampal synaptosomes across three postnatal timepoints (P0, P7, P35) in heterozygous Trio knockout (HET) and wildtype (WT) animals (N=60 post-QC). It covers outlier removal, TMM normalisation, PCA/MDS quality control, surrogate variable analysis (SVA) for latent variation, and differential expression analysis using voom/limma-edgeR with age-stratified contrasts. Downstream analyses include GO gene set enrichment (ClusterProfiler GSEA), overrepresentation analysis (gprofiler2), and preparation of gene sets for MAGMA analysis against neuropsychiatric GWAS data (psychENCODE), including mouse-to-human ortholog mapping via biomaRt. Visualisations include volcano plots, expression trajectory plots, and NES heatmaps across timepoints.

Key packages: edgeR, limma, sva, clusterProfiler, gprofiler2, biomaRt, ggplot2, pheatmap
