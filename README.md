# Employee Performance Analytics

## Overview

This project analyzes an Employee Performance Analytics dataset, consisting of features from 930 employees, to determine their suitability for specific projects. The primary objective is to build a semi-supervised model that clusters and predicts whether a selected employee would be a good fit for a project.

## Business Problem

With the increasing complexity of projects and the varying skill sets of employees, selecting the right candidates for project teams is crucial for ensuring success. This analysis aims to optimize project assignment by accurately predicting employee performance.

## Dataset

The dataset comprises various features related to employee performance, including but not limited to:

- Employee demographics
- Job-related metrics
- Past performance evaluations
- Skill sets

## Objectives

1. Build a semi-supervised machine learning model to cluster and predict employee suitability for projects.
2. Evaluate the performance of different classification models.
3. Identify the best model based on accuracy for inclusion of employees in projects.

## Model Performance

The project evaluates several classification algorithms and their performance on both training and testing datasets:

| Model                          | Training Accuracy | Test Accuracy |
|--------------------------------|-------------------|---------------|
| Logistic Regression            | 0.67              | 0.64          |
| Random Forest Classifier       | 1.00              | 0.74          |
| Decision Tree Classifier       | 0.74              | 0.69          |
| K-NN Classifier               | 0.76              | 0.68          |
| Gaussian Naive Bayes          | 0.65              | 0.64          |
| Multinomial Naive Bayes       | 0.68              | 0.65          |
| AdaBoost Classifier           | 0.73              | 0.76          |
| XGBoost Classifier            | 1.00              | 0.71          |

### Evaluation

- **Random Forest Classifier** and **XGBoost Classifier** demonstrated perfect training accuracy but showed a degree of overfitting, with significant differences in accuracy between training and test sets.
- The **AdaBoost Classifier** achieved the highest test accuracy among the models tested, indicating better generalization.

## Conclusion

The analysis highlights the importance of selecting the right model and tuning it for better performance. The findings can assist in creating targeted strategies for employee project assignments and overall improved resource allocation.

## Getting Started

### Prerequisites

- Python 3.x
- Required libraries:
  - pandas
  - numpy
  - scikit-learn
  - xgboost

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/employee-performance-analytics.git
