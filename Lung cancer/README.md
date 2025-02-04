# Lung Cancer Prediction using Machine Learning

---

## Table of Contents
1. [Description](#description)
2. [Models and Hyperparameter Tuning](#models-and-hyperparameter-tuning)
3. [Results](#results)
4. [Conclusion](#conclusion)

---

## Description
This project focuses on predicting lung cancer using various machine learning models. The models are trained and evaluated using **hyperparameter tuning** and **cross-validation** techniques to ensure robust performance.

---

## Models and Hyperparameter Tuning
The following machine learning models were used, and their hyperparameters were tuned using **GridSearchCV**:

| **Model**                     | **Best Parameters**                                                                 | **Best Score** | **Test Accuracy** |
|-------------------------------|-------------------------------------------------------------------------------------|----------------|-------------------|
| Logistic Regression           | `{'C': 10, 'solver': 'liblinear'}`                                                 | 0.9439         | 0.9748            |
| Decision Tree                 | `{'max_depth': None, 'min_samples_split': 10}`                                     | 0.9300         | 0.9328            |
| K-Nearest Neighbors           | `{'n_neighbors': 3, 'weights': 'distance'}`                                        | 0.8964         | 0.9580            |
| Gaussian Naive Bayes          | `{}`                                                                               | 0.9188         | 0.9580            |
| Multinomial Naive Bayes       | `{'alpha': 1}`                                                                     | 0.9244         | 0.9748            |
| Support Vector Classifier     | `{'C': 0.1, 'kernel': 'linear'}`                                                  | 0.9355         | 0.9916            |
| Random Forest                 | `{'max_depth': 10, 'n_estimators': 200}`                                           | 0.9439         | 0.9916            |
| Multi-Layer Perceptron        | `{'activation': 'tanh', 'hidden_layer_sizes': (100,), 'solver': 'adam'}`          | 0.9383         | 0.9916            |
| Gradient Boosting             | `{'learning_rate': 0.1, 'max_depth': 3, 'n_estimators': 200}`                     | 0.9355         | 0.9832            |

---

## Results
The models achieved the following accuracies on the test set:

| **Model**                     | **Test Accuracy** |
|-------------------------------|-------------------|
| Logistic Regression           | 0.9748            |
| Decision Tree                 | 0.9328            |
| K-Nearest Neighbors           | 0.9580            |
| Gaussian Naive Bayes          | 0.9580            |
| Multinomial Naive Bayes       | 0.9748            |
| Support Vector Classifier     | 0.9916            |
| Random Forest                 | 0.9916            |
| Multi-Layer Perceptron        | 0.9916            |
| Gradient Boosting             | 0.9832            |

---

## Conclusion
The Support Vector Classifier, Random Forest, and Multi-Layer Perceptron achieved the highest test accuracy of 99.16%, making them the best-performing models for this dataset. Hyperparameter tuning and cross-validation were critical in optimizing model performance.
