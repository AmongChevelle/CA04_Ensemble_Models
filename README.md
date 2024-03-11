# CA04_Ensemble_Models

## Overview

This project involves the use of ensemble models to analyze salary data obtained from the Census Bureau. The analysis aims to predict whether individuals earn more or less than $50K per year based on seven demographic variables. This assignment follows up on a previous analysis (CA03), utilizing the same dataset but focusing on ensemble methods to improve prediction accuracy and model performance.

## Data Source

The dataset is reused from CA03, featuring demographics and salary information:

- **Number of target classes:** 2 ('>50K' and '<=50K') [Labels: 1, 0]
- **Number of attributes (Columns):** 7
- **Number of instances (Rows):** 48,842

Data can be accessed at the following URL:
[https://github.com/ArinB/MSBA-CA-03-Decision-Trees/blob/master/census_data.csv?raw=true](https://github.com/ArinB/MSBA-CA-03-Decision-Trees/blob/master/census_data.csv?raw=true)

## Objectives

1. **Data Preparation:** Utilize the provided path to load the dataset. Split the data into training and test sets based on a specific column in the dataset. Ensure data cleaning and transformations are applied as done in CA03.

2. **Finding Optimal Value of a Key Ensemble Method Hyper-parameter:** Analyze the effect of the number of estimators on model performance. This involves plotting Accuracy vs. n_estimators and AUC vs. n_estimators graphs to find the optimal number of estimators.

3. **Building Ensemble Models:**
   - Train a Random Forest Model with the dataset. Explore the model's behavior and find an optimal number of estimators from the set [50, 100, 150, 200, 250, 300, 350, 400, 450, 500].
   - Repeat the analysis using AdaBoost, Gradient Boost, and XGB Classifiers.

4. **Performance Comparison:** Compare the best values of Accuracy and AUC for the four models (Random Forest, AdaBoost, Gradient Boost, XGB) and document the findings in a table.

## Deliverables

- A fully functional and executed Jupyter notebook.
- This README file documenting the project overview, data source, objectives, and analysis steps.

## Installation and Usage

Ensure you have Jupyter Notebook or JupyterLab installed to run the `.ipynb` file. Dependencies include `pandas`, `numpy`, `matplotlib`, `sklearn`, and `xgboost`. Install these packages via pip or conda if not already installed.

```bash
pip install pandas numpy matplotlib scikit-learn xgboost
```

To run the notebook:

1. Clone the repository or download the `.ipynb` file and this README to your local machine.
2. Open the notebook in Jupyter Notebook/Lab.
3. Execute the cells in order to reproduce the analysis.
