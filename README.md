# IBM HR Analytics Employee Attrition & Performance
This repository presents an end-to-end HR analytics project focused on employee attrition, based on the IBM HR Attrition dataset. The objective is to analyze, model, and predict which employees are most at risk of leaving, using modern data science and machine learning techniques. Business impact, cost analysis, and actionable strategies are included.  The best solution utilizes a Random Forest classifier with robust ROC-AUC, and addresses business impact with actionable strategies. All code, visuals, project summaries, and model artifacts are included for applied HR analytics and reproducible research.

## Table of Contents

- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Dataset Description](#dataset-description)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Modeling & Methodology](#modeling--methodology)
- [Business Impact & Recommendations](#business-impact--recommendations)
- [Directory Structure](#directory-structure)
- [How to Run](#how-to-run)
- [Dependencies](#dependencies)
- [Authors](#authors)

---

## Project Overview

Employee attrition is a critical business challenge. This project tackles the problem by performing:

- Data cleaning and preprocessing
- Exploratory data analysis (EDA) and visualization
- Feature engineering (binning, label encoding, log transforms, etc.)
- Model training with Logistic Regression and Random Forest classifiers
- Model evaluation using accuracy, recall, precision, ROC-AUC, and visual diagnostics
- Feature importance analysis
- Advanced cross-tabulations and statistical testing
- Business impact simulation (cost-benefit analysis)

## Key Features

- 📊 **Comprehensive EDA**: Attrition patterns by job role, income, age, gender, and more
- 🤖 **ML Pipelines**: StandardScaler/OneHotEncoder, class-imbalanced stratification, ROC curve comparison
- 🔥 **Best Model**: Random Forest (ROC-AUC ≈ 0.81), robust to class imbalance
- 🏆 **Feature Importance**: Key attrition drivers summarized for actionable HR insights
- 💡 **Business Recommendations**: Retention strategies and estimated financial savings
- 💻 **Reproducible Notebooks**: Clean, modular Jupyter code for custom HR analytics

## Dataset Description

Uses the canonical IBM HR Analytics Employee Attrition & Performance dataset. Features include:

- Demographics (Age, Gender, Marital Status, Education, etc.)
- Job details (Job Role, Department, Years at Company, OverTime, etc.)
- Compensation (Monthly Income, Stock Options, etc.)
- Job Satisfaction, Performance Ratings

## Exploratory Data Analysis

Visualizations included:
- Attrition rate by Job Role and Department
- Monthly Income distribution for attrition/no-attrition
- Correlation heatmaps of all variables
- Advanced crosstabs, chi-square significance testing

## Modeling & Methodology

- Data split: Stratified train/test (70/30)
- Preprocessing: StandardScaler for numeric, OneHotEncoder for categorical variables
- Model selection: Logistic Regression, Random Forest, evaluated via ROC-AUC
- Pipeline and model artifacts saved in `/models/`
- Feature importances extracted and interpreted

## Business Impact & Recommendations

- Estimated annual cost of attrition
- Projected savings from reducing attrition rates
- Recommendations: address overtime, targeted retention, salary reviews for at-risk roles
├── IBMHR.ipynb # Main Jupyter notebook (analysis & modeling)
├── IBM_Project_Report.pdf # Professional project report (PDF)
├── models/ # Saved model pipelines (.pkl)
├── charts/ # Key visualizations (ROC, EDA, feature importance, etc.)
├── data/ # Raw and processed datasets (if distributable)
└── README.md # This file


## How to Run

1. Clone this repository:
    ```
    git clone <repo-url>
    cd ibm-hr-analytics-attrition
    ```

2. (Recommended) Set up a new virtual environment and install dependencies:
    ```
    python -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt
    ```

3. Run the Jupyter notebook:
    ```
    jupyter notebook IBMHR.ipynb
    ```

4. Review visualizations, metrics, and saved model pipelines.

## Dependencies

- Python 3.8+
- pandas, numpy, scikit-learn, seaborn, matplotlib, scipy, jupyter

Install directly with:
pip install pandas numpy scikit-learn seaborn matplotlib scipy jupyter


## Authors

Thaduru Sathwik Reddy

## License

This project is licensed for educational and non-commercial use. IBM HR Analytics Employee Attrition & Performance dataset © IBM.

