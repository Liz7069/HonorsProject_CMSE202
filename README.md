# HonorsProject_CMSE202
This is Github repository for CMSE202 honors project


# Advertising Spend vs Sales Prediction (Machine Learning Project)

## Overview
This project explores the relationship between advertising spend and sales using machine learning models. The goal is to understand how different advertising channels (TV, Radio, Newspaper) influence sales and to evaluate whether machine learning models can capture these relationships effectively.

This project is part of a course project and serves as a project update demonstrating data preprocessing, exploratory analysis, and model development.

---

## Dataset
The dataset used in this project contains advertising budgets across three channels:
- TV
- Radio
- Newspaper

and the corresponding:
- Sales

The data is loaded from a CSV file (`advertising.csv`).

---

## Objectives
The main goals of this project are:
- Explore the relationship between advertising spend and sales
- Perform data cleaning and preprocessing
- Visualize patterns in the data
- Build and evaluate machine learning models
- Compare model performance

---

## Methods

### 1. Data Preprocessing
- Checked for missing values
- Converted data types if necessary
- Prepared features and target variables

### 2. Exploratory Data Analysis (EDA)
- Scatter plots to observe relationships
- Correlation analysis between variables
- Identification of trends across advertising channels

### 3. Machine Learning Models
The following models were implemented:
- Linear Regression (baseline model)
- Random Forest Regressor

### 4. Model Evaluation
Models were evaluated using:
- Mean Squared Error (MSE)
- R² Score

---

## Results
- TV advertising shows the strongest relationship with sales
- Radio has moderate impact
- Newspaper has weak or minimal impact

The Random Forest model generally performs better than Linear Regression in capturing nonlinear patterns.

---

## Files in this Repository

- `Project Update.ipynb`  
  Main notebook containing all code, analysis, and visualizations

- `advertising.csv`  
  Dataset used for this project

- `README.md`  
  Project description and documentation

---

## How to Run

1. Clone the repository:
```bash
git clone <your-repo-link>
