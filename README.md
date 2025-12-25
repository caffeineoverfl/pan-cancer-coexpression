# Pan-Cancer Co-Expression Analysis

## Overview
This project analyzes the co-expression patterns of tumor suppressor genes (TSGs) and oncogenes (OGs) across multiple human cancers using public RNA-Seq datasets. Conserved modules and hub genes are identified and functionally annotated.

## Datasets
- TCGA RNA-Seq: BRCA, LUAD, COAD (via recount3)
- COSMIC Cancer Gene Census: TSGs and OGs
- Optional: GTEx normal tissue for comparison

## Pipeline
1. Download raw data (`scripts/download_data.py`)
2. Preprocess data (`scripts/preprocess_data.py`)
3. Compute co-expression networks (`scripts/coexpression.py`)
4. Detect conserved modules (`scripts/module_analysis.py`)
5. Visualize results (`notebooks/04_visualization.ipynb`)

## Environment
Install dependencies using Conda:
```bash
conda env create -f environment.yml
conda activate pan-cancer-coexpression
