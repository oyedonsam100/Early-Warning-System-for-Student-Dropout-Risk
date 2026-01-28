📚 Student At-Risk Analysis
Overview

This project analyzes student performance to identify students at risk of failing. Using a public dataset, we perform data cleaning, exploratory data analysis (EDA), feature engineering, and predictive modeling to provide actionable insights for schools and educational planners.

The objective is to prioritize interventions for students most likely to struggle, enabling data-driven decisions that can improve outcomes.

Business Problem

Failing students can have long-term academic and social consequences. The goal of this project is to:

Identify students most at risk of failing.

Determine the factors driving poor performance.

Provide actionable insights for teachers and administrators.

Data

The dataset contains student demographics, academic performance, and lifestyle factors:

Features: age, sex, family background, study time, alcohol consumption, past failures, absences, etc.

Target: at_risk (binary – 1 = at risk, 0 = safe).

Data source: Student Performance Dataset

Feature Engineering

We derived six key features to capture student risk patterns:

Feature	Description
grade_trend	Change in grades across periods
has_failed_before	Indicator if student had prior failures
chronic_absence	High number of absences
alcohol_risk	Combined weekday/weekend alcohol consumption
family_support_score	Proxy for family support based on guardian/family info
high_study_commitment	High study time relative to peers
Exploratory Data Analysis

At-Risk Students: ~33% of students flagged as at risk.

Key Insights:

Students with chronic absences and prior failures are most likely to be at risk.

Family support and study habits significantly influence performance.

(You can include sample EDA plots here, e.g., grade distribution or alcohol vs performance)

Model Building

Two models were trained to predict at-risk students:

Model	Accuracy	Precision	Recall	F1-score
Logistic Regression	0.747	0.688	0.423	0.524
Random Forest	0.772	0.667	0.615	0.640

Observations:

Random Forest captures more at-risk students (higher recall) — critical for prioritizing interventions.

Logistic Regression offers interpretability through coefficients, while Random Forest gives a non-linear feature importance view.

Feature Importance Comparison


Comparison of Logistic Regression coefficients vs Random Forest feature importance.

Recommendations

Prioritize interventions for students with:

High chronic absences

Low grades or negative grade trends

High alcohol consumption

Low family support

Use Random Forest predictions to flag at-risk students early and guide support programs.

Next Steps

Explore other models: XGBoost, Gradient Boosting for performance improvement.

Build a dashboard for school administrators to visualize at-risk students.

Incorporate longitudinal data to track intervention outcomes over time.

Contact

Connect with me on LinkedIn www.linkedin.com/in/samuel-oyedokun-b41895142
 to discuss this project or collaborations in educational analytics.
