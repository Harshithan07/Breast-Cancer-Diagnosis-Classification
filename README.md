# Breast Cancer Diagnosis Classification – Predictive Modeling using WDBC Dataset

## ABOUT THE PROJECT:
This project aimed to build machine learning models to predict whether a tumor is malignant or benign based on diagnostic features from the Wisconsin Diagnostic Breast Cancer (WDBC) dataset. The primary goal was to identify a high-recall model suitable for medical decision-making where minimizing false negatives is critical.


## USE CASE EXPLANATION:
In clinical diagnostics, early and accurate identification of cancerous tumors is essential to enable timely intervention. This project falls under the healthcare analytics and biomedical machine learning domains. The model supports medical practitioners, radiologists, and automated diagnostics tools by providing a second opinion for breast cancer prediction using patient tumor feature data.


## HOW IT IS BUILT AND FULL WORKING:

1. Data Source: 
- UCI WDBC dataset containing 569 samples, 30 numeric features derived from tumor cell nuclei images (mean, standard error, worst values).

2. Data Processing:

- Removed non-predictive ID column.

- Applied Min-Max scaling to standardize feature ranges.

- Split into training/testing sets (80/20).

3. Model Development:

- Built and evaluated three classifiers:

   i. Logistic Regression (L1, LibLinear)

   ii. K-Nearest Neighbors (K=3,5,7,9)

   iii. Decision Tree (varied depth and split criteria)

- Performed hyperparameter tuning using GridSearchCV (5-fold).

- Generated classification reports and plotted learning curves to detect overfitting/underfitting.

4. Evaluation Metrics:

- Used Recall as the primary metric (due to healthcare domain).

- Also evaluated Accuracy, Precision, F1-score, ROC-AUC.


## OUTPUT AND RESULTS OR BENCHMARKS:

- Best model: Logistic Regression with L1 regularization

- Recall = 1.00 (100%), ROC-AUC = 0.997, F1-score ≈ 0.97

- KNN underperformed without scaling; Decision Tree showed overfitting at high depth.

- Final model prioritized recall to avoid missing malignant cases — a medically critical outcome.

## SKILLS, TOOLS:
Python, scikit-learn, GridSearchCV, Logistic Regression, KNN, Decision Tree, MinMaxScaler, ROC curve analysis, matplotlib, classification metrics

## KEYWORDS:
Healthcare analytics, breast cancer detection, supervised classification, machine learning in medicine, recall optimization, ROC-AUC, model evaluation, scikit-learn, diagnostic prediction, binary classification
