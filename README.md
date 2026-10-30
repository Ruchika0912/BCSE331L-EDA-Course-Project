# BCSE331L – Exploratory Data Analysis Course Project
## Analysis of Police Shooting Incidents in the USA (2015 – 2020)

**Student:** Ruchika Tuteja | **Register Number:** 23BDS0050

**Video demonstration:** [Paste your public video link here]

### Contents
| File | Description |
|---|---|
| `EDA_Project_Ruchika_Tuteja.ipynb` | Complete notebook, Phase I – III (Modules 2 to 7) |
| `EDA_Project_Report_23BDS0050.docx` | Final project report |

### What the notebook covers
| Phase | Module | Topics |
|---|---|---|
| I | 2 | Data loading, inspection, missing values, cleaning, feature engineering |
| I | 3 | Descriptive statistics, univariate (1D) analysis |
| II | 4 | Bivariate (2D), multivariate (3D) and correlation analysis |
| II | 5 | K-Means and hierarchical clustering |
| III | 6 | Principal Component Analysis (scree plot, loadings, biplot, 3D projection) |
| III | 7 | Logistic Regression classifier for signs of mental illness (confusion matrix, ROC-AUC, cross-validation, odds ratios) |

### Dataset
`shootings.csv` (4,895 rows, 15 columns), loaded directly from the faculty repository:
https://raw.githubusercontent.com/salemprakash/EDA/main/Data/shootings.csv

### How to run
Click the **Open in Colab** badge at the top of the notebook and choose *Runtime → Run all*. No local setup is needed.

Requirements if running locally: `pandas numpy matplotlib seaborn scikit-learn scipy`

### Key results
- **PCA:** PC1–PC3 explain 30.8% of the variance and 11 of 16 components are needed for 80%, so the variables share little common variance.
- **Logistic Regression:** ROC-AUC 0.71, recall 72% for the minority class (5-fold CV AUC 0.709 ± 0.012), compared with a majority-class baseline that detects no positive cases.
