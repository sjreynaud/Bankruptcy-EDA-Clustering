# Corporate Bankruptcy EDA and K-Means Clustering

## Overview
Brief description of the project:
- Large U.S. corporate bankruptcy dataset (78,682 firm-year observations).
- Full EDA + unsupervised k-means clustering (k = 2).
- Goal: segment firms by financial distress and approximate bankruptcy status.

## Repository structure
- `data/` – source data or data notes.
- `rmarkdown/` – full annotated R Markdown analysis.
- `reports/` – APA-style paper and knitted PDF.
- `slides/` – presentation slides.
- `code/` – reusable R scripts (EDA, clustering, evaluation).
- `docs/` – executive summary and methodology notes.

## Methods
Short bullets:
- Data preprocessing: type checks, missingness (none), outlier review.
- Scaling: z-score standardization of numeric variables.
- Feature engineering: `financial_stress_index = (total_liabilities / total_assets) - (net_income / total_assets)`.
- Clustering: k-means with k = 2 on scaled numeric features.
- Evaluation: accuracy, precision, recall, F1-score on mapped clusters.

## Key results
- Accuracy: 93.8%
- Precision: 93.8%
- Recall: 99.9%
- F1-score: 0.968

## How to run
1. Install required R packages (`tidyverse`, `skimr`, `GGally`, `caret`, `janitor`, `yardstick`, `factoextra`, etc.).
2. Place `american_bankruptcy.csv` in `data/`.
3. Open `rmarkdown/Implement_EDA_Clustering_Bankruptcy.Rmd` in RStudio.
4. Knit to PDF or run chunks interactively.

## Author
Sidney J. Reynaud, Jr.  
Links to LinkedIn and GitHub.
