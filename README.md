# BioPrinciple-A2

## Overview

This document provides details about **Assignment 2** titled "Gene Expression Analysis and Interpretation." It is written in R Markdown and performs a comprehensive analysis of a gene expression dataset, focusing on the following tasks:

- Dataset preparation and untarring.
- Differential expression analysis.
- Pathway enrichment analysis.
- Principal Component Analysis (PCA).
- Heatmap visualization of gene expression data.
- Survival modeling using Lasso regression.

The analysis leverages a breast cancer dataset sourced from cBioPortal and employs R programming along with Bioconductor packages to achieve its objectives.

## Prerequisites

### Software Requirements

To execute this R Markdown file, ensure your system meets the following requirements:

- **R version**: 4.0 or higher
- **RStudio**: Recommended for a streamlined experience

### Required R Packages

Before running the analysis, install the following R packages:

```R
install.packages(c("tidyverse", "ggplot2", "survival", "glmnet"))
BiocManager::install(c("cBioPortalData", "TCGAbiolinks", "ComplexHeatmap", "clusterProfiler"))
```

### Dataset Requirements

- Download the dataset from **cBioPortal**.
- Ensure the dataset is correctly formatted and stored in the specified directory (`C:/Users/asus/Downloads`). 

## Execution Instructions

Follow these steps to execute the R Markdown file:

1. **Clone or Download the Repository**
   - Save the R Markdown file (`Assignment_2.Rmd`) into your working directory.

2. **Open the File**
   - Use RStudio to open the `Assignment_2.Rmd` file.

2. **Dataset Requirements Check**
   - Ensure the dataset (`brca_tcga_pan_can_atlas_2018.tar.gz`) is downloaded in Downloads folder.
   - Set the value of downloads_path variable in the first code chunk with the path of the Downloads folder according to the user's system. (For example - "C:/Users/asus/Downloads")

3. **Run the Code**
   - Execute each code chunk sequentially.
   - Ensure that the required packages are installed before running the script. Install them if prompted.

4. **Output**
   - The analysis produces the following outputs:
     - Visualizations, including PCA plots and heatmaps
     - Summary tables of enriched pathways and survival model performance metrics.

## Key Sections

### 1. Dataset Preparation

This section initializes the environment, sets up file paths, and extracts the dataset for further analysis.

### 2. Differential Expression Analysis

This step identifies genes that are significantly expressed between different groups.

### 3. Pathway Enrichment

The identified genes are used to perform enrichment analysis, uncovering significant biological pathways.

### 4. Visualization

- **PCA**: Reduces dimensionality and visualizes group differences.
- **Heatmap**: Displays clustering of gene expression data.

### 5. Survival Modeling

Lasso regression is applied to predict survival outcomes based on gene expression profiles.

## Troubleshooting

- **Missing Dataset**: Ensure the dataset is downloaded and placed in the correct folder.
- **Package Errors**: Reinstall packages and verify version compatibility.

---

**Author:** Pranay Jain  
**Date:** 2024-12-20

