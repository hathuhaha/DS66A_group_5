# Predicting Customer Insurance Purchase Behavior

Project for the **Statistical Learning** course, College of Technology, National Economics University (NEU).

## General Information

- **Class:** DS66A
- **Group:** 5
- **Supervisor:** Dr. Thien Van Luong
- **Date:** Hanoi, October 30, 2026

## Team Members

| No. | Full Name | Student ID |
|-----|-----------|------------|
| 1 | Hà Thu Hà | 11248476 |

## Research Topic

**Predicting Customer Insurance Purchase Behavior**

This project builds supervised machine learning models to predict which customers own a caravan insurance policy (target variable `CARAVAN`), using the **COIL 2000 (CoIL Challenge 2000)** dataset.

### Key Points

- **Data:** 5,822 labelled customers for training and 4,000 for evaluation, each described by 85 input variables. Only about 6% of customers own a caravan policy, so accuracy is not a useful metric.
- **Exploratory data analysis (EDA):** chi-square tests with Benjamini–Hochberg correction, removal of 8 redundant columns, and one-hot encoding of 6 variables.
- **Models:** Logistic Regression, K-Nearest Neighbours, Decision Tree, Random Forest, and Support Vector Machine, with hyperparameters tuned on a validation set.
- **Metrics:** Average Precision (AP) as the primary metric, ROC-AUC as a complementary measure.
- **Results:** Logistic Regression with L1 regularization performed best. On the official test set it achieved AP = 0.1532 and ROC-AUC = 0.7278, better than random ranking but still modest.
