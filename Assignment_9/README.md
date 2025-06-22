# Assignment 9 - Unsupervised Learning on Wholesale Customers Dataset

## Overview

This project applies unsupervised learning techniques to cluster customer purchasing behavior using the **Wholesale Customers Dataset**. The goal is to identify natural segments in the customer base for better decision-making in marketing and distribution.

## Dataset

**Source**: UCI Machine Learning Repository  
**Link**: [Wholesale Customers Data](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers)

**Features**:
  - Fresh, Milk, Grocery, Frozen, Detergents_Paper, Delicassen
**Categorical (Dropped)**:
  - Channel, Region

## Methods Used

**Preprocessing**:
  - Removed categorical features
  - Standardized numerical values

**Clustering Algorithms**:
  - KMeans (Optimal k=3 based on silhouette score)
  - Agglomerative Clustering (used for comparison)

**Dimensionality Reduction**:
  - PCA (2 components) for visualization

**Evaluation Metrics**:
  - Silhouette Score
  - PCA Scatter Plots
  - Dendrograms

## Results

**Best model**: KMeans with 3 clusters (Silhouette Score: **0.458**)
**Agglomerative Clustering** performed poorly in comparison (Score: **0.239**)
- PCA visualization showed well-separated clusters

## Deployment & Monitoring (Hypothetical)

- Model would be deployed in a real-time microservice to segment new customers.
- Challenges addressed:
  - Latency
  - Scalability
  - Drift over time
- Monitoring strategies include:
  - Drift detection
  - Regular retraining pipelines
  - Dashboarding with latency and scoring metrics

## Files

- `Assignment9.ipynb`: Main analysis notebook
- `Assignment9_Report.pdf`: Two-page summary report with visuals and findings
- `README.md`: Project overview and instructions

