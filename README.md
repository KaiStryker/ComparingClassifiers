# Comparing Classifiers on Bank Marketing Dataset

## Overview
This project focuses on comparing the performance of several classifiers, namely K-Nearest Neighbors (KNN), Logistic Regression, Decision Trees, and Support Vector Machines (SVM), using a dataset related to marketing bank products over the telephone. The data originates from a Portuguese banking institution and includes results from multiple marketing campaigns.

## Dataset
The dataset is sourced from the UCI Machine Learning repository and encompasses 17 campaigns from May 2008 to November 2010. It includes a variety of features from bank client data, last contact information, and social and economic context attributes, alongside the target variable indicating if a client subscribed to a term deposit.

### Features
- **Bank client data**: Age, job, marital status, education, default, housing, loan
- **Last contact of the current campaign**: Contact communication type, last contact month and day of the week, duration
- **Other attributes**: Number of contacts performed during and before this campaign, outcome of the previous marketing campaign
- **Social and economic context attributes**: Employment variation rate, consumer price index, consumer confidence index, euribor 3 month rate, number of employees

### Target Variable
- **y**: Has the client subscribed to a term deposit? (binary: 'yes', 'no')

## Objective
The goal is to determine which classifier is most effective for predicting whether a client would subscribe to a term deposit.

## Methodology
1. **Data Preparation**: Encoding categorical features and splitting the dataset into training and testing sets.
2. **Baseline Model**: Establishing a baseline performance using the most frequent class.
3. **Model Building and Comparison**: Training and scoring Logistic Regression, KNN, Decision Trees, and SVM models, comparing their accuracy and fit time.
4. **Improvements**: Experimenting with feature engineering, hyperparameter tuning, and adjusting performance metrics to enhance model performance.
5. **Resampling Techniques**: Utilizing oversampling and undersampling to address class imbalance and improve model predictions.

## Results
- The Logistic Regression model showed notable performance improvements with resampling techniques, leading to more balanced and less biased predictions.
- Precision-Recall and ROC curves were plotted to evaluate model performance, showing that the Logistic Regression model, with resampling, outperformed other classifiers in terms of F1 score and balanced accuracy.

## Conclusion and Recommendations
The Logistic Regression model, after applying resampling techniques, emerged as the best performing model based on scoring and fit time. To further optimize this model and achieve closer to baseline accuracy, focusing on different feature selection methods and hyperparameter testing is recommended.

## Future Work
- Further exploration of feature engineering to identify the most impactful features.
- Extensive hyperparameter optimization to fine-tune model performance.
- Evaluation of additional classifiers and ensemble methods for comparison.
