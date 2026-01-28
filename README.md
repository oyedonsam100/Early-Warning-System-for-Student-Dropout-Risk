# 📚 Early Warning System for Student Dropout Risk

## Overview
This project analyzes student performance to identify those at risk of failing. Using the Student Performance Dataset, we perform **data cleaning**, **exploratory data analysis (EDA)**, **feature engineering**, and **predictive modeling** to provide actionable insights for schools, teachers, and educational planners.

The objective is to prioritize interventions for students most likely to struggle, enabling **data-driven decisions** that improve educational outcomes.

---

## Business Problem
Failing students can face long-term academic and social consequences. Schools need a system to:

- Identify students at risk of failing.
- Determine the key factors driving poor performance.
- Provide actionable insights for teachers and administrators.
- Optimize educational resources and prioritize interventions.

---

## Data
The dataset contains **student demographics, academic performance, and lifestyle factors**:

**Features include:**

- `age`, `sex`, `family background`, `study time`, `alcohol consumption`, `past failures`, `absences`, etc.

**Target variable:** 

- `at_risk` (binary: 1 = at risk, 0 = safe)

**Data Source:** [Student Performance Dataset](https://archive.ics.uci.edu/ml/datasets/Student+Performance)

---

## Feature Engineering
We derived six key features to capture student risk patterns:

| Feature | Description |
|---------|-------------|
| `grade_trend` | Change in grades across periods |
| `has_failed_before` | Indicator if student had prior failures |
| `chronic_absence` | High number of absences |
| `alcohol_risk` | Combined weekday/weekend alcohol consumption |
| `family_support_score` | Proxy for family support based on guardian/family info |
| `high_study_commitment` | High study time relative to peers |

---

## Exploratory Data Analysis (EDA)
- **At-Risk Students:** ~33% of students flagged as at risk.
- **Key Insights:**
  - Students with chronic absences and prior failures are most likely to be at risk.
  - Family support and study habits significantly influence performance.

**Example Plots:**

**At-Risk Students Distribution**
![At-Risk Distribution](Model%20Performance%20Comparison.png)

**Feature Importance Comparison**
![Feature Importance](Feature%20Importance%20Comparison.png)

---

## Model Building
Two models were trained to predict at-risk students:

| Model | Accuracy | Precision | Recall | F1-score |
|-------|---------|----------|--------|----------|
| Logistic Regression | 0.747 | 0.688 | 0.423 | 0.524 |
| Random Forest | 0.772 | 0.667 | 0.615 | 0.640 |

**Observations:**
- Random Forest captures more at-risk students (higher recall) — critical for prioritizing interventions.
- Logistic Regression provides interpretability via coefficients, while Random Forest captures non-linear relationships.

---

## Recommendations
Schools should prioritize interventions for students with:

- **High chronic absences**
- **Negative grade trends**
- **High alcohol consumption**
- **Low family support**

Use **Random Forest predictions** to flag at-risk students early and guide support programs.

---

## Next Steps
- Explore other models: **XGBoost, Gradient Boosting** for better performance.
- Build a **dashboard for school administrators** to visualize at-risk students.
- Incorporate **longitudinal data** to track intervention outcomes over time.

---

## Contact
Connect with me on LinkedIn: [Samuel Oyedokun](https://www.linkedin.com/in/samuel-oyedokun-b41895142) to discuss this project or collaborations in educational analytics.

---

## About
This project demonstrates how **data science and predictive modeling** can improve student outcomes and optimize educational resource allocation.

