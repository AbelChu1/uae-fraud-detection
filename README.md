# UAE E-Commerce Fraud Detection

Supervised binary classification project to detect fraudulent transactions 
in the UAE e-commerce market using machine learning.

## Overview

This project was built as part of my Machine Learning coursework. 
It applies supervised classification techniques to a dataset of 100,000 
synthetic UAE e-commerce transactions to identify fraudulent activity.

The dataset contains 40+ features including payment details, device 
information, geographic indicators, and behavioral signals. 
Only 8.2% of transactions are fraudulent, making this a highly 
imbalanced classification problem.

## Models Trained

- Logistic Regression
- Decision Tree
- Random Forest
- SGD Classifier
- Soft Voting Ensemble
- KNN and SVM (tested, excluded at scale)

## Key Results

| Model               | Binary F1 | ROC-AUC |
|---------------------|-----------|---------|
| Logistic Regression | ~0.21     | ~0.68   |
| Decision Tree       | ~0.22     | ~0.66   |
| Random Forest       | ~0.21     | ~0.68   |
| SGD Classifier      | ~0.21     | ~0.68   |
| Voting Ensemble     | ~0.21     | ~0.68   |

Best model: Decision Tree (highest Binary F1 after tuning)

## What I Learned

- Why accuracy is a deceptive metric on imbalanced datasets
- How a dummy classifier achieves 91.8% accuracy by predicting 
  "not fraud" every time, while detecting zero fraud cases
- How to use GridSearchCV with Stratified K-Fold cross-validation 
  for systematic hyperparameter tuning
- Why f1_binary is the correct scoring metric for imbalanced 
  fraud detection tasks

## Project Structure

| File | Description |
|------|-------------|
| `Assignment_1_Fraud_Detection.ipynb` | Full notebook with code and analysis |
| `Report.pdf` | Written report covering methodology and findings |

## Dataset

The dataset is publicly available on Kaggle:
[UAE E-Commerce Fraud Dataset](https://www.kaggle.com/datasets/atharvasoundankar/uae-e-commerce-fraud)

## Tools and Libraries

Python, Scikit-Learn, Pandas, NumPy, Matplotlib, Seaborn, KaggleHub

## Run in Google Colab

[Open In Colab](https://colab.research.google.com/drive/1DavbBfFYLKjXQvw9ljm9v1Ui0Y2J6qte?usp=sharing)

## Author

Abel Chuchu  









