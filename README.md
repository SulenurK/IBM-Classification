**Machine Learning Project: Predicting Machine Failures**
This project was developed as part of the Supervised Machine Learning: Classification course in the IBM Machine Learning Specialization. The goal of this project is to predict machine failures using machine learning techniques, enabling proactive maintenance and optimizing operational efficiency.

**Project Overview**
Objective: Predict machine failures based on operational data to minimize downtime and reduce maintenance costs.
Dataset: The Predictive Maintenance Dataset (AI4I 2020) was used, which includes 10,000 observations of machine conditions such as temperature, rotational speed, torque, and tool wear.
Target Variable: Binary classification (Machine Failure: 0 for no failure, 1 for failure).

**Key Steps**
**Data Exploration and Preprocessing:**
Explored data distributions using histograms, boxplots, and correlation heatmaps.
Handled imbalanced data using StratifiedShuffleSplit.
Applied log transformation to normalize skewed features.
Encoded categorical features using one-hot encoding.

**Model Training and Evaluation:**
Trained and evaluated three classifier models: Decision Tree, Random Forest, and XGBoost.
Used 5-fold cross-validation for robust performance evaluation.
Focused on recall as the primary metric to maximize failure detection.

**Fine-Tuning the Best Model:**
Performed grid search to optimize hyperparameters for the XGBoost Classifier.
Achieved a recall of 69.12% and an F1 score of 0.7769.
Analyzed feature importance to identify key drivers of machine failures (e.g., Torque, Tool Wear).

**Key Findings:**
Extreme values of Torque [Nm] and Tool Wear [min] are strong predictors of failures.
The XGBoost Classifier outperformed other models, balancing predictability and interpretability.
