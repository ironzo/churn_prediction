### Churn Prediction with SMOTE
This repository contains examples of how to implement SMOTE (Synthetic Minority Oversampling Technique) to predict customer churn using various machine learning models. The dataset used for this project was sourced from a Coursera Data Science competition.

#### Introduction
Imbalanced datasets are a common challenge in binary classification tasks, such as churn prediction, fraud detection, spam filtering, and rare disease prediction. Models trained on such datasets may become biased towards the majority class, leading to poor recall metrics. To address this issue, we use SMOTE to generate synthetic samples for the minority class, improving the model's ability to identify it.

#### Models
I trained several machine learning models on the preprocessed data, both with and without SMOTE. The models include:
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Random Forest
Additionally, I applied threshold tuning to the models trained with SMOTE to optimize their performance.

#### Evaluation
The models were evaluated based on accuracy, precision, recall, and F1 score.

#### Conclusions
- SMOTE generally improves recall across all models but often at the cost of reduced precision and accuracy.
- Threshold tuning after applying SMOTE can help balance precision and recall, often resulting in better F1 scores.
- Logistic Regression with SMOTE and threshold tuning achieved the highest F1 score (44.74) among all models and methods.
- Simple models (without SMOTE) tend to have higher accuracy but lower recall, indicating they may be less effective at identifying the minority class.

