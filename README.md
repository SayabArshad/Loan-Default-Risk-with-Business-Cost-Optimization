# Task-4-Loan-Default-Risk-with-Business-Cost-Optimization

## ✅ Task Objective
To predict loan default risk and reduce overall business loss by optimizing the model decision threshold based on a cost-benefit framework.

## 🔍 Our Approach
- Loaded and explored the `application_train.csv` dataset from Home Credit.
- Performed data cleaning: handled missing values, categorical encodings, and standardized numerical features.
- Used Logistic Regression and CatBoost Classifier to build classification models.
- Defined asymmetric business costs:
  - False Negatives (missed defaulters) cost the business significantly more than False Positives (false rejections).
- Optimized classification threshold using a custom cost function that minimized total expected loss.
- Evaluated models using ROC-AUC, precision-recall curves, and a cost-based confusion matrix.
- Applied SHAP values and CatBoost’s built-in feature importance to interpret model decisions.

## 📊 Results and Findings
- CatBoost outperformed Logistic Regression, especially on imbalanced data.
- Optimizing the decision threshold resulted in a significant reduction in business cost compared to default threshold (0.5).
- Important risk features included:
  - Credit Bureau history
  - External risk scores
  - Type of income and employment
- The risk scoring system is now more aligned with real-world costs, improving the institution’s financial performance.
