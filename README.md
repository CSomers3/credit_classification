# credit_classification
Credit classification on imbalanced data (DataLink 2023 Submission)

### Executive Summary

The German Credit dataset is a widely used dataset in the machine learning community,
consisting of 798 entries with 20 categorical and continuous attributes. The objective of the
dataset is to predict whether a person applying for a bank loan is a good or bad credit risk.
The dataset is imbalanced, with more than double the number of good credit observations.
Exploratory data analysis shows that variables such as duration, amount, age, and savings
status are critical predictor variables. Therefore, we conclude that both customer
characteristics and loan specifications are important for this task.

To prepare the data for modelling, we use one-hot and binary encoding for feature
engineering. To simplify the model, we apply two feature selection techniques: Chi-Squared
testing and Recursive Feature Elimination. Accounting for the data imbalance we test both
SMOTE and Random Oversampling techniques. We then evaluate a broad range of
classification models and find that the final Random Forest model has an accuracy of 79%
and a more crucial metric, macro F1-score, of 66% on out-of-sample data.

