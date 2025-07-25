# 📉 Customer Churn Analysis & Prediction in Retail Banking

## 🧭 Objective
The goal of this project is to analyze customer churn behavior in a retail bank and build interpretable machine learning models to predict which customers are likely to leave. Through a mix of exploratory data analysis (EDA), modeling, and evaluation, this project aims to:

- Identify key demographic and behavioral drivers of churn
- Predict churn with reliable performance
- Derive actionable insights to support retention strategies

---

## 🔍 Key Questions Explored
- What demographic and behavioral traits are most associated with churn?
- Can we reliably predict customer churn?
- Which features contribute most to customer exits?
- How can we balance precision and recall using threshold tuning?

---

## 📊 Tools & Techniques

| Category          | Tools / Methods                                 |
|-------------------|--------------------------------------------------|
| **EDA & Viz**     | Pandas, Matplotlib, Seaborn                     |
| **Modeling**      | Logistic Regression, Decision Tree, Random Forest, XGBoost |
| **Evaluation**    | Accuracy, Precision, Recall, F1-Score, ROC-AUC, PR-AUC |
| **Interpretability** | Coefficients, Odds Ratios, Feature Importance |
| **Threshold Tuning** | Precision-Recall Curve, Business-Driven Thresholding |

---

## 📁 Project Structure
├── churn_analysis.ipynb # Main notebook with EDA + Modeling
├── README.md # Project summary and documentation
└── (Optional) requirements.txt # List of dependencies (if needed)


---

## ✅ Summary of Findings

- **Age**, **IsActiveMember**, and **Number of Products** are key drivers of churn.
- **Germany** as a geography saw a notably higher churn rate.
- **Inactivity** is a strong churn signal across all segments.
- **Logistic Regression**, **Random Forest**, and **XGBoost** offered competitive performance, with Random Forest leading on overall metrics.

---

## 📈 Model Comparison (Highlights)

| Model              | Accuracy | Precision | Recall | F1 Score | PR AUC |
|--------------------|----------|-----------|--------|----------|--------|
| Logistic Regression | 76.5%    | 0.42      | 80.7%  | 0.55     | 0.60   |
| Random Forest       | 84.5%    | 0.42      | 82.7%  | 0.56     | 0.69   |
| XGBoost             | 83.7%    | 0.42      | 81.7%  | 0.55     | 0.69   |

> Thresholds tuned to ensure: **Recall ≥ 80% and Precision ≥ 42%**

---

## 📌 Takeaways

- For **analytical interpretability**, Logistic Regression is a strong baseline.
- For **higher recall and precision balance**, Random Forest and XGBoost are more robust.
- Threshold tuning helps prioritize **recall** for churn mitigation, especially in business contexts where missing a churned customer is costlier than acting on a false positive.

---

