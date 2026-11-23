# Bonus Project B: Loan Risk Assessment System

## Problem Statement
This project builds an automated machine learning system to predict loan approval risks for credit applicants, enabling financial institutions to make data-driven lending decisions and minimize default rates.

## Dataset
- **Name:** Analytics Vidhya Loan Prediction Dataset
- **Source:** Analytics Vidhya GitHub Repository
- **Link:** https://raw.githubusercontent.com/subashgandyer/datasets/master/loan_train.csv
- **Rows / Columns:** 614 rows, 13 columns

## Tools Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

## Workflow
1. Data Collection
2. Data Cleaning & Imputation (Mode for Categorical, Median for Numerical, Sentinel Category for Credit History)
3. Exploratory Data Analysis (EDA) - Categorical countplots, continuous boxplots, and numeric correlation matrix
4. Feature Engineering (Created total_income and loan_income_ratio features, scaled numerical columns)
5. Model Building (Logistic Regression, Tuned Decision Tree Classifier, Random Forest Classifier)
6. Evaluation (Accuracy, Precision, Recall, F1-Score, and ROC-AUC curves)
7. Insights & Recommendations

## Results
- **Model:** Random Forest Classifier (Best Performing Model)
- **Key Metric(s):** Accuracy = 0.8699, Precision = 0.8791, Recall = 0.9412, F1-Score = 0.9091, ROC-AUC = 0.8546
- **Top Factors / Drivers:**
  1. **Credit History**: Strongest indicator of loan approval status.
  2. **Total Household Income**: Synthesized combination of applicant and coapplicant income.
  3. **Loan Income Ratio**: Normalized scale of requested loan relative to overall earnings.

## Screenshots
![Model Evaluation - Confusion Matrices](Images/confusion_matrices.png)
![Model Evaluation - ROC Curve](Images/roc_curve.png)

## Future Improvements
- Explore advanced gradient boosting frameworks like XGBoost or LightGBM for minor metric optimization.
- Apply Synthetic Minority Over-sampling Technique (SMOTE) to mitigate any potential class imbalance in rejected loans.
- Deploy the trained classifier as a simple interactive web API using Flask or FastAPI.

## Author
[Edwin Nkengafac] | [https://www.linkedin.com/in/edwin-nkengafac-27137a2b3/]
