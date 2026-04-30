# Advertising Spend vs. Sales Prediction
### CMSE 202 Honors Project — Machine Learning with the Advertising Dataset

---

## Research Question

How does advertising spend across different marketing channels (TV, Radio, Newspaper) affect sales, and which channel has the strongest impact?

---

## Overview

This project explores the relationship between advertising spend and sales using machine learning models. Two models — Linear Regression and Random Forest Regressor — are trained and compared to understand how different advertising channels influence sales and to evaluate which approach captures those relationships more effectively.

---

## Motivation

Companies invest heavily in marketing, but not all advertising channels are equally effective. Understanding which channels drive the most sales can help businesses allocate budgets more efficiently and maximize return on investment. This project applies machine learning techniques from CMSE 202 to a real-world marketing dataset to answer that question quantitatively.

---

## Dataset

**Source:** [Advertising Dataset — Kaggle](https://www.kaggle.com/datasets/ashydv/advertising-dataset)

- **200 observations**, each representing a market
- **Features:** TV, Radio, and Newspaper advertising budgets (in $thousands)
- **Target:** Sales (in thousands of units)

---

## Methodology

### 1. Data Preprocessing
- Loaded dataset from `advertising.csv`
- Checked for missing values and confirmed data types
- Prepared feature matrix (`TV`, `Radio`, `Newspaper`) and target variable (`Sales`)

### 2. Exploratory Data Analysis (EDA)
- Histograms of all four variables to understand distributions
- Scatter plots for each channel vs. Sales to identify relationships
- Correlation analysis to quantify channel-sales associations

### 3. Model Training
Both models trained on an **80/20 train-test split** (`random_state=42`):

| Model | Type | Notes |
|---|---|---|
| Linear Regression | Parametric baseline | Interpretable coefficients |
| Random Forest Regressor | Ensemble (200 trees) | Captures non-linear patterns |

### 4. Model Evaluation
- **R² Score** — proportion of variance explained
- **Mean Squared Error (MSE)** — average prediction error

---

## Results

| Model | R² Score | MSE |
|---|---|---|
| Linear Regression | 0.906 | 2.91 |
| **Random Forest** | **0.955** | **1.40** |

**Key findings:**
- **TV** is the strongest predictor of sales (feature importance: **0.844**)
- **Radio** has a moderate secondary effect (importance: **0.136**)
- **Newspaper** shows negligible predictive value (importance: **0.019**)
- Random Forest outperforms Linear Regression by capturing non-linear relationships
- Residual analysis confirms no systematic model bias

---

## Files in this Repository

| File | Description |
|---|---|
| `Project_Update.ipynb` | Main notebook: all code, analysis, and visualizations |
| `advertising.csv` | Dataset used for this project |
| `README.md` | Project description and documentation |
| `CMSE202_honors_revised_ppt.pptx` | Presentation slides |

> 📧 **Note:** A recorded video walkthrough of the presentation was submitted separately via email to the professor.

---

## Tools & Libraries

- Python 3
- `pandas` — data loading and preprocessing
- `numpy` — numerical operations
- `matplotlib` — visualization
- `scikit-learn` — model training and evaluation

---

## How to Run

1. **Clone the repository:**
```bash
   git clone <your-repo-link>
   cd <repo-folder>
```

2. **Install dependencies:**
```bash
   pip install pandas numpy matplotlib scikit-learn
```

3. **Launch the notebook:**
```bash
   jupyter notebook Project_Update.ipynb
```

4. Make sure `advertising.csv` is in the same directory as the notebook.

---

## Course

**CMSE 202 — Computational Modeling Tools and Techniques**  
Michigan State University — Honors Section
