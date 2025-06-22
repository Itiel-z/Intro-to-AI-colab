# Student Performance Classification

This project applies machine learning techniques to predict whether students will pass or fail based on demographic and academic features. The dataset used is from the UCI Student Performance repository.

## Dataset

- Source: [Student Performance Data](https://raw.githubusercontent.com/amankharwal/Website-data/master/student-mat.csv)
- 395 student records
- 33 features (e.g., age, study time, absences, parent education)
- Target variable: `pass` (binary classification based on final grade `G3`)

## Problem Statement

Predict whether a student will pass (`1`) or fail (`0`) based on various academic and personal factors. This is a binary classification problem.

## Project Structure

- **Exploratory Data Analysis (EDA)**: Checked for class distribution and feature correlations.
- **Data Preprocessing**:
  - Performed label binarization on the pass column
  - Removed raw grade columns (G1, G2, G3)
  - One-hot encoded categorical features
  - Scaled numeric features
- **Modeling**:
  - Logistic Regression
  - Random Forest Classifier
- **Evaluation**:
  - Accuracy, Precision, Recall, F1-score
  - Confusion Matrix
  - Suggested: ROC Curves
- **Model Deployment (Design)**:
  - Export trained model using `joblib`
  - REST API using Flask or FastAPI
  - Real-time input handling and monitoring strategies proposed

## Results

 Model                 Accuracy  Precision  Recall   F1 Score 
 Logistic Regression     0.71       0.74     0.87      0.80
 Random Forest           0.66       0.68     0.90      0.78     

**Logistic Regression performed best overall** based on balanced metrics.
