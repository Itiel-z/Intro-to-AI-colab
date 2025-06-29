# Credit Card Fraud Detection using Machine Learning

This project addresses the real-world problem of detecting fraudulent transactions from credit card data using classification algorithms. It is part of an AI/ML course project, 
showcasing the application of supervised learning models and model evaluation strategies.

## Project Structure

- `Final_project.ipynb`: Jupyter notebook containing the full data analysis, preprocessing, modeling, and evaluation.
- `creditcard.csv`: Dataset used for training and evaluation (not included in this repo, available from [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)).
- `README.md`: Project overview and instructions.
- `report.pdf`: Project report summarizing the methodology and findings.

## Dataset

- **Source**: [Kaggle Credit Card Fraud Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Records**: 284,807 transactions
- **Fraudulent transactions**: Only 492 (highly imbalanced)
- **Features**: PCA-transformed features V1–V28, `Amount`, and `Class` (target)

## Models Used

- Logistic Regression (with `class_weight='balanced'`)
- Random Forest Classifier
- Support Vector Machine (SVM)

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## Libraries

- Pandas
- NumPy
- Scikit-learn
- Seaborn
- Matplotlib


##  Running the Project

1. Clone the repository or open in Google Colab.
2. Upload `creditcard.csv` to your environment.
3. Run all cells in `Final_project.ipynb`.

