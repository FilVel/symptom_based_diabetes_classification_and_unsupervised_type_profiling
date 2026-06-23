# Symptom-based Diabetes Classification and Unsupervised Type Profiling
Project for a University Machine Learning course

## Abstract

Driven by the critical clinical importance of the early detection of type 1 diabetes, this project proposes a multi-stage machine learning framework using a symptom-based clinical dataset to address the absence of explicit disease-type labels.

Utilising data from 520 patients collected at the Sylhet Diabetes Hospital, which tracks 16 categorical and numerical attributes (including age, gender, polyuria, polydipsia, and sudden weight loss) mapped to a binary target, the methodology establishes a dual-layer approach.

In the first stage, a supervised binary classification pipeline evaluates tabular classifiers—such as Decision Trees and Random Forests—to accurately distinguish between healthy and diabetic cohorts, mathematically prioritizing classification over regression to target discrete diagnostic labels.

In the second stage, an unsupervised clustering layer utilizing K-Means (k=2) is applied strictly to the predicted positive instances. This allows for an empirical evaluation of whether latent clinical signatures naturally partition into two distinct clusters aligning with known epidemiological profiles of type 1 (acute, early-onset) and type 2 diabetes.

To ensure methodological rigor, data preparation is managed via an end-to-end scikit-learn transformer pipeline to prevent data leakage during categorical encoding and feature scaling, while stratified k-fold cross-validation and systematic hyperparameter tuning are implemented to mitigate overfitting risks on the 520-instance sample.

## Dataset
https://www.kaggle.com/datasets/arshaprasad/diabetes-dataset/data
