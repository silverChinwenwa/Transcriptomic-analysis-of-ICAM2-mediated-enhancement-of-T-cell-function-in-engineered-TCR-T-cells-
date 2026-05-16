# Transcriptomic-analysis-of-ICAM2-mediated-enhancement-of-T-cell-function-in-engineered-TCR-T-cells-
_RNA-seq differential gene expression analysis comparing_
The dataset is publicly available via GEO accession: GSE330057

**Overview**

This project performs a full RNA-seq differential gene expression analysis comparing:
_TCRT_ICAM2 condition
CRT control condition_
The goal is to identify significantly dysregulated genes and uncover their associated biological processes using Gene Ontology enrichment.

**My process**
Data Pre-processing
Log transformation of expression values
Separation of experimental groups (CRT vs TCRT)
Differential Expression Analysis
Computation of: Log Fold Change (logFC), p-values
Multiple testing correction using Benjamini-Hochberg (FDR)
Filtering Significant Genes
Adjusted p-value < 0.05|logFC| > 1
Visualization
Volcano plots (significance vs fold change)
Heatmap of top differentially expressed genes
Functional Enrichment Analysis

**Tool**
GSEApy (Enrichr API)
Database: GO Biological Process 2023
Organism: Human
Gene ID Processing
Cleaning and formatting gene identifiers
Conversion to gene symbols (via MyGene API)

**Libraries**
Python
Pandas, NumPy
Matplotlib, Seaborn
Statsmodels
GSEApy
MyGene

**Key Findings**
ICAM2 overexpression significantly alters gene expression profiles in TCR-T cells.
Several genes associated with T cell memory and stemness (e.g., FOXO1, CCR7, TCF7) show differential regulation.
Enrichment analysis highlights pathways related to: Immune activation, Cell survival, Metabolic regulation

**Interpretation**
The results support the hypothesis that ICAM2 promotes a stem-like, long-lived T cell phenotype, which is associated with enhanced anti-tumor activity.
This aligns with the ICAM2 → mTORC2 → FOXO1 pathway, suggesting improved persistence and functionality of engineered T cells.
