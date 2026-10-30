# BCSE331L – Exploratory Data Analysis Course Project
## Analysis of Police Shooting Incidents in the USA (2015 – 2020)

**Student:** Ruchika Tuteja | **Register Number:** 23BDS0050

**Video demonstration:** https://drive.google.com/file/d/1Rd7IG-ofBdlU-vfSrXVQNkE7dq8cELiE/view?usp=share_link

### Contents
| File | Description |
|---|---|
| `EDA_Project_Ruchika_Tuteja.ipynb` | Complete notebook, Phase I – III (Modules 2 to 7) |
| `EDA_Project_Report_23BDS0050.docx` | Final project report |

### What the notebook covers
| Phase | Module | Topics |
|---|---|---|
| I | 2 – Data Transformation | Replacing values, deduplication, missing data (deletion, imputation, MLE), discretization and binning |
| I | 3 – Correlation Analysis and Time Series Analysis | Univariate, bivariate, multivariate and correlation analysis; time-based indexing, resampling, grouping |
| I/II | 4 – Data Summarization and Visualization | Summary measures, contingency tables and chi-square tests, n-D analysis, dot chart, outlier detection |
| II | 5 – Clustering Algorithms | K-Means, hierarchical agglomerative clustering, outlier detection using clustering |
| III | 6 – Dimensionality Reduction | PCA (scree plot, loadings, biplot, 3D projection) and SVD |
| III | 7 – Model Development and Evaluation | Logistic Regression classifier: accuracy, precision/recall/F1, ROC-AUC, cross-validation, odds ratios |

### Dataset
`shootings.csv` (4,895 rows, 15 columns), loaded directly from the faculty repository:
https://raw.githubusercontent.com/salemprakash/EDA/main/Data/shootings.csv

### How to run
Click the **Open in Colab** badge at the top of the notebook and choose *Runtime → Run all*. No local setup is needed.

Requirements if running locally: `pandas numpy matplotlib seaborn scikit-learn scipy`

### Key results
- **PCA:** PC1–PC3 explain 30.8% of the variance and 11 of 16 components are needed for 80%, so the variables share little common variance.
- **Logistic Regression:** ROC-AUC 0.71, recall 72% for the minority class (5-fold CV AUC 0.709 ± 0.012), compared with a majority-class baseline that detects no positive cases.
