
# Research Methodology
## Heart Disease Prediction Using Machine Learning

## 1. Refined Research Question

How effectively can Logistic Regression and Random Forest classify the presence or absence of heart disease using clinical attributes from the UCI Cleveland Heart Disease dataset?

The main objective is to compare two supervised classification algorithms and evaluate their performance using appropriate classification metrics.

## 2. Dataset Description

**Dataset Name:** Heart Disease (Cleveland Subset)

**Source:** UCI Machine Learning Repository

**Dataset Link:** https://archive.ics.uci.edu/dataset/45/heart

**Dataset Size:** 303 instances

**Predictive Features:** 13

**Original Target Variable:** num

The dataset contains clinical and demographic information about patients. Its predictive features include age, sex, chest pain type, resting blood pressure, cholesterol, fasting blood sugar, resting ECG results, maximum heart rate, exercise-induced angina, ST depression, slope, number of major vessels, and thal.

### Target Variable

The original target variable, num, contains values from 0 to 4.

For this experiment, it will be converted into a binary target:

- 0 = No heart disease
- 1 = Heart disease present (original values 1, 2, 3, or 4)

### Dataset Limitations

- The dataset contains only 303 instances, which is relatively small for machine learning experiments.
- The ca and thal features contain missing values.
- The dataset is based on historical clinical records and may not represent current or diverse patient populations.
- The experiment will use only the Cleveland subset, so its results may not generalize to other populations or hospitals.

## 3. Data Cleaning Plan

The following steps will be performed:

1. Load the Cleveland dataset using Pandas.
2. Assign the appropriate column names based on the UCI documentation.
3. Inspect the dataset shape, data types, and statistical summary.
4. Identify missing values, including values represented by '?'.
5. Convert missing-value markers into proper NaN values.
6. Check for duplicate records.
7. Handle missing numerical and categorical values using suitable imputation methods.
8. Verify that the target variable is correctly converted into binary form.

Missing-value imputation will be fitted using the training data only to avoid data leakage.

## 4. Feature Engineering Plan

The following feature preparation steps will be used:

1. Convert the original num target into a binary classification target.
2. Separate the 13 predictive features from the target variable.
3. Identify categorical and numerical features.
4. Apply appropriate encoding to categorical features when required.
5. Apply StandardScaler to numerical features for Logistic Regression.
6. Use the same training and testing split for both models.

All preprocessing operations will be performed through a Scikit-learn pipeline where appropriate.

## 5. Machine Learning Models

Two classification algorithms will be used.

### 5.1 Logistic Regression

Logistic Regression will be used as the baseline classification model. It is relatively simple and interpretable and can estimate the probability of a binary outcome.

Feature scaling will be applied because the model can be affected by differences in feature scales.

### 5.2 Random Forest Classifier

Random Forest is an ensemble learning algorithm that combines multiple decision trees. It can model nonlinear relationships and feature interactions.

It will be used to compare its classification performance with Logistic Regression.

## 6. Model Evaluation Metrics

Both models will be evaluated using the same test dataset.

The following metrics will be used:

### Accuracy

Measures the proportion of correctly classified observations among all observations.

### Precision

Measures how many predicted positive cases are actually positive.

### Recall

Measures how many actual positive cases are correctly identified.

### F1-score

Provides a harmonic mean of precision and recall.

### Confusion Matrix

Shows true positives, true negatives, false positives, and false negatives.

Recall will receive particular attention because missing a patient with heart disease can be an important concern in a screening-oriented classification task.

## 7. Experimental Procedure

The experiment will follow these steps:

1. Load and inspect the dataset.
2. Clean missing values and duplicate records.
3. Create the binary target variable.
4. Separate features and target.
5. Split the data into training and testing sets using stratified sampling.
6. Apply preprocessing to the training data.
7. Train Logistic Regression.
8. Train Random Forest.
9. Evaluate both models using the same test set.
10. Compare the evaluation results.

A fixed random state will be used to make the experiment reproducible.

## 8. Expected Outcome

The experiment is expected to provide a comparison between Logistic Regression and Random Forest on the Cleveland Heart Disease dataset.

The actual performance of both models will be determined from the experimental results rather than assumed in advance.

The study will also help identify the limitations of using a small, historical clinical dataset for heart disease classification.
