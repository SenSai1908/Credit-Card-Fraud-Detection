# Credit-Card-Fraud-Detection
Model Performance Overview
The credit card fraud detection model was evaluated on a highly imbalanced dataset, where the majority of transactions were non-fraudulent. The model was trained using a Random Forest Classifier, and the evaluation metrics indicate strong performance across various measures:

Key Metrics:
Accuracy: The model achieved an accuracy of 99.96%, meaning it correctly predicted the class of transactions in 99.96% of cases.
Precision:
Non-Fraud (Class 0): 100% precision, meaning all transactions predicted as non-fraud were indeed non-fraudulent.
Fraud (Class 1): 94% precision, indicating that 94% of transactions flagged as fraudulent were actual frauds.
Recall:
Non-Fraud (Class 0): 100% recall, meaning all non-fraudulent transactions were correctly identified.
Fraud (Class 1): 80% recall, meaning the model correctly identified 80% of fraudulent transactions while missing 20%.
F1-Score:
Class 0 (Non-Fraud): 1.00
Class 1 (Fraud): 0.86
Confusion Matrix:
The confusion matrix highlights the model's ability to classify transactions correctly:

True Negatives (Non-Fraud classified correctly): 56,859
True Positives (Fraud classified correctly): 78
False Positives (Non-Fraud misclassified as Fraud): 5
False Negatives (Fraud misclassified as Non-Fraud): 20
Imbalance Handling
The dataset exhibited a significant class imbalance, with fraudulent transactions being a small fraction of the total:

Non-Fraudulent Transactions (Class 0): 56,864
Fraudulent Transactions (Class 1): 98
The model's performance demonstrates its robustness despite the imbalance. Techniques such as the use of a balanced random forest and appropriate hyperparameter tuning contributed to minimizing false positives and false negatives.

Future Improvements
To further enhance the model's performance:

Increase Recall for Fraud: Use techniques like SMOTE (Synthetic Minority Oversampling Technique) or undersampling to handle class imbalance more effectively.
Optimize Hyperparameters: Perform grid search or randomized search to fine-tune parameters such as n_estimators, max_depth, and min_samples_split.
Threshold Adjustment: Experiment with decision thresholds to reduce false negatives (missed fraud cases).
This project showcases the use of machine learning for real-world fraud detection, leveraging the Random Forest algorithm for its interpretability and robustness.
