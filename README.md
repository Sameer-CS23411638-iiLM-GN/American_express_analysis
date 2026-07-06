# 💳 American Express Customer Profitability Ranking Framework

> A business-driven profitability ranking model developed for the **American Express Campus Challenge 2026**.

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow)
![NumPy](https://img.shields.io/badge/NumPy-Numerical-green)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-red)

---

## 📌 Project Overview

Financial institutions need to identify their most valuable customers to optimize retention strategies, reward programs, and credit risk management.

In this challenge, a dataset containing **500,000 anonymized American Express cardmembers** with **23 behavioral attributes** was provided.

Since the actual profitability labels were unavailable, the objective was to **design an explainable profitability framework** capable of ranking customers from the most profitable to the least profitable using business logic, financial reasoning, and data analytics.

---

## 🎯 Business Objective

Develop a transparent scoring framework that estimates customer profitability by balancing:

- 💰 Revenue Generation
- 🎁 Reward & Benefit Costs
- ⚠️ Credit Risk
- 🤝 Customer Engagement

The final output is a ranked list of all customers based on predicted profitability.

---

## 📊 Dataset

- **500,000 Customers**
- **23 Anonymous Features**
- Behavioral
- Financial
- Engagement
- Risk
- Reward Usage

No personally identifiable information (PII) was used.

---

# 🛠 Project Workflow

```
Raw Dataset
      │
      ▼
Exploratory Data Analysis
      │
      ▼
Missing Value Treatment
      │
      ▼
Outlier Handling
      │
      ▼
Rank Normalization
      │
      ▼
Feature Engineering
      │
      ▼
Profitability Framework
      │
      ▼
Customer Ranking
```

---

# 📈 Exploratory Data Analysis

Performed:

- Missing Value Analysis
- Correlation Analysis
- Feature Distribution Analysis
- Outlier Detection
- Rank Transformation
- PCA Exploration
- Statistical Profiling

---

# ⚙️ Data Cleaning

Business-driven preprocessing was applied.

| Problem | Solution |
|----------|----------|
| Missing Spend | Filled with 0 |
| Missing Benefit Usage | Filled with 0 |
| Missing Risk | Median Imputation |
| Highly Sparse Features | Removed |
| Extreme Outliers | Winsorization (1st–99th Percentile) |

---

# 🚀 Feature Engineering

Five business-oriented features were created.

### Customer Value

Represents revenue generation based on spend and revolving balance.

---

### Engagement Score

Captures customer relationship strength using:

- Website activity
- Product depth
- Customer interactions

---

### Premium Efficiency

Measures how efficiently customers generate revenue relative to premium benefits consumed.

---

### Risk Adjusted Spend

Discounts spending by expected credit risk.

---

### Expected Loss

Estimated as:

```
Expected Loss = Risk Probability × Revolving Balance
```

---

# 🧮 Final Profitability Framework

```
Final Score =
0.40 × Customer Value
+ 0.20 × Engagement Score
+ 0.20 × Premium Efficiency
+ 0.20 × Risk Adjusted Spend
− 0.40 × Expected Loss
```

The framework prioritizes customers with:

- High Revenue
- Strong Engagement
- Efficient Premium Usage
- Low Credit Risk

---

# 📊 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook

---



# 📌 Key Insights

- Spending variables were highly correlated.
- Customer profitability depends on balancing revenue and risk.
- Missing values often represented genuine business behavior rather than incomplete data.
- Rank normalization significantly improved robustness against skewed distributions.
- Explainable business rules produced an interpretable profitability framework.

---

# 📈 Business Impact

This framework can support:

- Customer Segmentation
- Credit Line Optimization
- Premium Product Targeting
- Retention Strategy
- Reward Cost Optimization
- Risk Monitoring

---

# 🔮 Future Improvements

- XGBoost
- LightGBM
- CatBoost
- Learning-to-Rank Models
- SHAP Explainability
- Ensemble Ranking

---

# 👨‍💻 Author

**Sameer**

Computer Science Engineer

Passionate about

- Data Science
- Machine Learning
- Business Analytics
- Artificial Intelligence

---

⭐ If you found this project interesting, consider giving it a Star.
