# Bank Loan Default Prediction

## Overview
This project predicts the likelihood of a customer defaulting on a bank loan using financial and demographic features. It employs a Random Forest Classifier 
and includes explainability with SHAP, as well as fairness and ethical evaluations.


## Libraries Used
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- SHAP (SHapley Additive exPlanations)

## Dataset Description

The dataset contains information about bank customers and their financial status, with the goal of predicting whether a customer will default on a loan.
***Features***
- age: Age of the customer in years
- ed: Education level (ordinal scale, 1 = low to 5 = high)
- employ: Number of years the customer has been employed
- address: Number of years at the current address
- income: Annual income in thousands of dollars
- debtinc: Debt-to-income ratio (percentage)
- creddebt: Amount of credit card debt in thousands of dollars
- othdebt: Other debts in thousands
- default: Target variable: 1 = defaulted, 0 = did not default

### Number of Records
- **Total Entries**: 850
- **After Removing Missing Targets**: 700
  
## How to Run

1. Clone the repository or upload the code to a Jupyter/Colab notebook.
2. Ensure required libraries are installed:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn shap
