# CampusPulse – Student Life Analysis (Task 1)

This repository contains the solution to **Task 1: The CampusPulse Initiative** from the Machine Learning Coding Week 2025, organized by the Coding Club, IIT Guwahati.

## 📌 Problem Statement

CampusPulse is a data science initiative to explore lifestyle, academic performance, and social behavior patterns among students at IIT Guwahati. One of the central questions is:

**Can we predict if a student is likely to be in a romantic relationship based on lifestyle and academic data?**

## ✅ Completed Levels

### 🔍 Level 1: Variable Identification Protocol
Three anonymized features (`Feature_1`, `Feature_2`, `Feature_3`) were statistically analyzed:
- `Feature_1` was identified as **Age** (based on min/max and correlation with failures)
- `Feature_2` as **Study Time** (correlated positively with G1, G2, G3)
- `Feature_3` as **Extrovertedness** (positively correlated with alcohol and going out, negatively with grades)

### 🧹 Level 2: Data Integrity Audit
Handled missing values using a combination of:
- Dropping (for `famsize`)
- Median imputation (`Fedu`, `age`, `studytime`, `extrovert`)
- Domain-based filling (e.g., setting `traveltime` to 0, `higher` to 0, etc.)

### 📊 Level 3: Exploratory Insight Report
Explored the following questions:
1. Do students in relationships have more absences?
2. Does family relationship quality impact romantic involvement?
3. Is there a link between mother’s education and paid classes?
4. How does living in urban vs rural areas affect alcohol consumption?
5. Does travel time influence final grades?

Used `boxplot`, `violinplot`, `scatterplot`, and `countplot` with proper interpretation.

### 🤖 Level 4: Relationship Prediction Model
Built and evaluated two models:
- **Logistic Regression**: Accuracy ~67%
- **Random Forest**: Accuracy ~60%

Performed encoding, feature engineering, and tested both full feature and reduced-feature models.

### 🧠 Level 5: Model Interpretation
- Applied **SHAP** for global feature importance.
- Used **SHAP force plots** to explain predictions for individual students.

## 🛠️ Libraries Used
- Python, pandas, numpy
- seaborn, matplotlib
- scikit-learn, shap

---

**Name:** Ritesh Raj Singh  
**Roll Number:** 240101079  
