# Customer-Response-Prediction

## Objective
Build a scalable machine learning pipeline in **PySpark** to predict whether a customer will respond positively or negatively to a **marketing promotion campaign**. The project showcases how to implement end-to-end data preparation, model training, and evaluation in a distributed computing environment.

This pipeline is inspired by and adapted from a previously completed traditional Scikit-learn workflow, highlighting how to reproduce and scale it using PySpark's MLlib.

---

## Workflow Summary

- Data cleaning and Data Exploration Analysis in the first notebook for feature engineering
- Load and prepare customer annual and monthly data
- Feature engineering using `VectorAssembler` and `StandardScaler`
- Temporal-based train/test split
- Fit and tune multiple ML models:
  - Logistic Regression (with L1 penalty)
  - Decision Tree
  - Random Forest
- Evaluate model performance using AUC and precision-recall metrics

---

## Problem Statement
**Predict whether a customer will respond positively or negatively to a promotional campaign** based on transactional history features using annual and monthly datasets

---

## Models Used
- **Logistic Regression (L1-regularized)**  
- **Decision Tree Classifier**  
- **Random Forest Classifier**

Each model is tuned using `CrossValidator` and `ParamGridBuilder` to maximize generalization performance.

---

## Results
- Logistic regression (L1-regularized) with Annual Data offered high interpretability and best generalization.

---

## Tools & Libraries
`PySpark` · `Spark MLlib` · `Pandas` · `Jupyter Notebooks` · `Databricks` · `Scikit-learn` (for comparison)

---

## References
- [Spark MLlib Docs](https://spark.apache.org/docs/latest/ml-guide.html)
- [Scikit-learn Pipeline Reference](https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html)

