
# Research Proposal

## 1. Research Title

Heart Disease Prediction Using Machine Learning Classification Algorithms

## 2. Introduction

Heart disease is one of the major health concerns worldwide. Early identification of heart disease can help healthcare professionals make better decisions.

Machine learning techniques can analyze clinical data and identify patterns that may help predict the presence of heart disease.

This project aims to explore machine learning classification algorithms for heart disease prediction using publicly available clinical data.

## 3. Research Question

How effectively can machine learning classification algorithms predict the presence of heart disease using clinical attributes?

## 4. Dataset Information

- Dataset Name: UCI Heart Disease Dataset
- Subset: Cleveland
- Total Records: 303
- Input Features: 13
- Source: UCI Machine Learning Repository

Dataset Link:
https://archive.ics.uci.edu/dataset/45/heart

The dataset contains clinical attributes such as age, sex, chest pain type, resting blood pressure, cholesterol, and maximum heart rate.

## 5. Research Objectives

1. To analyze clinical attributes related to heart disease.
2. To apply different machine learning classification algorithms.
3. To compare the performance of the selected algorithms.
4. To evaluate the models using standard classification metrics.

## 6. Proposed Methodology

The following machine learning algorithms will be used:

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier

The dataset will undergo basic preprocessing, including missing value handling and categorical feature encoding.

Model performance will be evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

## 7. Preliminary Literature Review

Two relevant research studies have been identified.


## 7. Literature Review

### Study 1: Noroozi et al. (2023)

**Paper Title:** Analyzing the impact of feature selection methods on machine learning algorithms for heart disease prediction

**Authors:** Zeinab Noroozi, Azam Orooji, and Leila Erfannia

**Publication:** Scientific Reports, 2023

**DOI:** https://doi.org/10.1038/s41598-023-49962-w

**Summary:**

This study investigated the impact of different feature selection methods on machine learning algorithms for heart disease prediction. The researchers used the Cleveland Heart Disease Dataset and evaluated sixteen feature selection techniques along with seven machine learning algorithms.

Their findings showed that feature selection could improve the performance of some algorithms, while it could reduce the performance of others. The study also highlighted the importance of selecting relevant features for better classification performance.

**Relevance to Our Research:**

This study helps us understand the importance of feature selection and algorithm comparison in heart disease prediction. It provides a useful foundation for our proposed comparative classification study.

### Study 2: Bouqentar et al. (2024)

**Paper Title:** Early heart disease prediction using feature engineering and machine learning algorithms

**Authors:** Mohammed Amine Bouqentar, Oumaima Terrada, Soufiane Hamida, Shawki Saleh, Driss Lamrani, Bouchaib Cherradi, and Abdelhadi Raihani

**Publication:** Heliyon, 2024

**DOI:** https://doi.org/10.1016/j.heliyon.2024.e38731

**Summary:**

This research focused on early heart disease prediction using feature engineering and machine learning algorithms. The researchers used Cleveland and Statlog heart disease datasets to compare several classification algorithms, including Logistic Regression, Decision Tree, Random Forest, Support Vector Machine, and K-Nearest Neighbors.

The study evaluated model performance using accuracy, precision, recall, F1-score, and AUC. It also applied hyperparameter tuning and cross-validation to analyze model performance.

**Relevance to Our Research:**

This study provides a useful reference for comparing different classification algorithms and evaluating their predictive performance. It supports our plan to compare Logistic Regression, Decision Tree, and Random Forest.

## 8. Research Gap and Proposed Contribution

Previous studies have explored different machine learning algorithms and feature selection techniques for heart disease prediction.

Our project will focus on a simple comparative analysis of three classification algorithms using the Cleveland Heart Disease Dataset.

The study will investigate how Logistic Regression, Decision Tree, and Random Forest perform under the same dataset and evaluation settings.

## 9. Proposed Methodology

The proposed workflow includes:

1. Dataset Collection
2. Data Inspection and Preprocessing
3. Missing Value Handling
4. Categorical Feature Encoding
5. Train-Test Split
6. Model Training
7. Model Performance Comparison

The selected algorithms are:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

The models will be evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

The original target variable will be converted into binary classes, where 0 represents no heart disease and values 1 to 4 represent the presence of heart disease.

## 10. Expected Outcome

The expected outcome is a comparative understanding of the performance of different machine learning classification algorithms for heart disease prediction.

The project will identify the strengths and limitations of the selected algorithms based on standard classification evaluation metrics.

## 11. References

1. Noroozi, Z., Orooji, A., & Erfannia, L. (2023). Analyzing the impact of feature selection methods on machine learning algorithms for heart disease prediction. Scientific Reports, 13, 22588. https://doi.org/10.1038/s41598-023-49962-w

2. Bouqentar, M. A., Terrada, O., Hamida, S., Saleh, S., Lamrani, D., Cherradi, B., & Raihani, A. (2024). Early heart disease prediction using feature engineering and machine learning algorithms. Heliyon, 10(19), e38731. https://doi.org/10.1016/j.heliyon.2024.e38731
