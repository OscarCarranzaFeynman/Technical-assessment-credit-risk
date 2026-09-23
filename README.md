# Credit Risk Analysis

Technical assessment focused on predicting customer credit risk through data
cleaning, exploratory data analysis, feature preparation, and supervised machine
learning.

## Project overview

The analysis compares Logistic Regression and Random Forest models for a binary
classification problem. Because the target is imbalanced, model evaluation goes
beyond accuracy and includes precision, recall, F1-score, ROC-AUC, and confusion
matrices.

## Repository structure

```text
.
├── data/          # Training and prediction datasets
├── notebooks/     # Exploratory analysis and model development
├── presentation/  # Project presentation
├── pyproject.toml # Project metadata and dependencies
└── uv.lock        # Reproducible dependency lockfile
```

## Methods and tools

- Data cleaning and exploratory data analysis
- Feature preparation and train/test splitting
- Logistic Regression
- Random Forest
- Model evaluation for imbalanced classification
- Python, Pandas, NumPy, Matplotlib, Seaborn, and Scikit-learn

## Getting started

This project uses [uv](https://docs.astral.sh/uv/) to manage Python and its
dependencies.

```bash
git clone https://github.com/OscarCarranzaFeynman/Technical-assessment-credit-risk.git
cd Technical-assessment-credit-risk
uv sync
uv run jupyter lab
```

Open `notebooks/credit_risk_analysis.ipynb` in JupyterLab and select the Python
environment created for the project if prompted.

## Data

The notebook expects the following local files:

```text
data/data_train.xlsx
data/data_test.xlsx
```

## Key findings

- Accuracy alone did not adequately describe performance because the target was
  imbalanced.
- Recall and ROC-AUC provided a more useful view of default-risk detection.
- Balanced models improved the identification of higher-risk customers.
