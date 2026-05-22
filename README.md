Gene Expression Pipeline — Microarray Analysis (GSE1000)


A complete, end‑to‑end gene expression analysis pipeline built in Python to analyze microarray data from the GEO dataset GSE1000.


Project Overview

This project demonstrates real‑world bioinformatics skills including data preprocessing, normalization, PCA, differential expression analysis, and visualization.

This pipeline investigates how biomaterial surface chemistry affects gene expression in human cells.
Using microarray data from GEO, the workflow:

Loads and cleans raw expression data

Applies log‑normalization and z‑scoring

Performs PCA to identify sample clustering

Runs differential expression analysis (log2FC + Welch’s t‑test)

Generates publication‑quality visualizations

Clusters top differentially expressed genes

This project is designed as a portfolio‑ready demonstration of computational biology skills for research labs, internships, and industry roles.

Repository Structure

Gene-expression-Pipeline/

│

├── pipeline.py              # Full analysis pipeline

├── data/                    # (Optional) GEO dataset or instructions

├── figures/                 # PCA, volcano plot, heatmap

└── README.md                # Project documentation


Methods & Workflow

1. Data Loading & Cleaning
Reads GEO series matrix file

Converts all values to numeric

Removes non‑numeric rows

2. Metadata Assignment
Maps each GSM sample to:

Surface type

Time point

3. Normalization
Log2 transform

Z‑score per gene

4. PCA
Identifies clustering patterns across surface types.

5. Differential Expression Analysis
log2 fold change

Welch’s t‑test

Ranked gene list

6. Volcano Plot
Highlights significantly up/down‑regulated genes.

7. Heatmap of Top DE Genes
Top 50 genes

Z‑scored expression

Color‑coded by surface type

📊 Key Visualizations
PCA Plot
Shows sample clustering by surface chemistry.

Volcano Plot
Highlights significantly regulated genes.

Heatmap
Top 50 differentially expressed genes across samples.

Key Visualizations

PCA Plot
Shows sample clustering by surface chemistry.

Volcano Plot
Highlights significantly regulated genes.

Heatmap
Top 50 differentially expressed genes across samples.

Biological Insights

Samples cluster strongly by surface type, indicating real biological structure.

Differential expression reveals distinct transcriptional responses between Aspartic Acid and Polystyrene surfaces.

Heatmap shows clear gene‑level separation across conditions.

This demonstrates that biomaterial chemistry can influence cellular gene expression programs.

Skills Demonstrated

Python (NumPy, Pandas, SciPy, Seaborn, Matplotlib)

Microarray data processing

Differential expression analysis

PCA and clustering

Data visualization

Debugging and pipeline design

Biological interpretation



Pavan Pancholi  
Bioinformatics & Computational Biology
UMBC

