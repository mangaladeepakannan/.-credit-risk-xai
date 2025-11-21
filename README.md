# .-credit-risk-xai
A complete Explainable AI (XAI) project for predicting credit risk using LightGBM, Optuna, SHAP, and LIME. Includes full preprocessing, model training, hyperparameter tuning, global and local interpretability, fairness analysis, and actionable underwriting insights.

# 🏦 Interpretable Credit Risk Assessment using SHAP & LIME  
A complete end-to-end Explainable AI (XAI) project for predicting loan default using advanced machine learning (LightGBM + Optuna) and interpreting the model using SHAP and LIME. Designed for high-stakes financial environments where transparency, fairness, and regulatory compliance are essential.

---

## 📌 Project Overview  
This project develops a robust credit-risk prediction model and explains how and why the model makes loan-approval decisions using modern interpretability frameworks.  
It is fully aligned with regulatory expectations (Basel III, EU AI Act, Responsible AI principles).

### **Key Objectives**
- Build and tune a high-performance classification model for loan default prediction.  
- Produce global and local explanations using **SHAP**.  
- Validate decision boundaries and per-customer decisions using **LIME**.  
- Compare explainability methods for fairness, bias, and compliance.  
- Convert insights into actionable recommendations for underwriting teams.

---

## 📂 Dataset  
This project uses the publicly available **Credit Risk Dataset** on Kaggle:

🔗 *https://www.kaggle.com/datasets/laotse/credit-risk-dataset*  

### **Target Variable**
- `loan_status` (1 = default, 0 = repaid)

### **Features**
Includes loan information, borrower demographics, and financial indicators.

---

## ⚙️ Tech Stack  
- **Python 3.8+**  
- **LightGBM** – Gradient boosting model  
- **Optuna** – Automated hyperparameter optimization  
- **SHAP** – Global and local explanations  
- **LIME** – Local instance explanations  
- **scikit-learn** – Preprocessing and metrics  
- **Matplotlib** – Visualizations  

---

## 🏗️ Project Workflow

### **1. Data Preprocessing**
- Handle missing values  
- One-hot encode categorical columns  
- Train/test split  
- Outlier and imbalance checks (optional)

### **2. Model Development**
- LightGBM classifier  
- Optuna tuning (20–50 trials recommended)  
- Evaluation metrics:  
  - ROC-AUC  
  - F1-score  
  - Classification report  
  - Confusion matrix

### **3. SHAP Explainability**
- Global summary plot  
- Top feature dependence plots  
- Local force plots (optional)

### **4. LIME Local Explainability**
- Explanation for individual customers  
- Comparison with SHAP values  
- Identify approval/denial rationale  
- Highlight fairness implications  

### **5. Deliverables**
All generated outputs are saved in the folder:


---
**Expected Deliverables**

1. Python/R Code Implementation (Plain Text)

The repository provides the complete machine learning pipeline in plain Python code, including:

Dataset preprocessing

Train/test split

LightGBM model training

Optuna hyperparameter tuning

SHAP global & local explainability

LIME per-instance explainability

Saving outputs (plots, HTML explanations, model artifacts)

The full implementation is located in:
credit_risk_project.ipynb

This script can be executed directly to reproduce all results.
✅ 2. Text-Based Report (≤1000 Words)

A clearly written analytical report summarizing:

Model Performance

ROC–AUC

F1-score

Classification report

Misclassification patterns

Interpretation of feature importance

SHAP vs. LIME Comparative Analysis

Strengths of SHAP for global interpretability

Strengths of LIME for case-level decision understanding

Consistencies and discrepancies between both explainability frameworks

Fairness & bias implications related to applicant subgroups

Regulatory compliance alignment (Basel III, Responsible AI guidelines)

The report is included in the repository as:

REPORT_shap_lime_analysis.txt


✅ 3. Text Output Containing LIME Explanations (5 Cases)

The project generates LIME explanations for:

2 high-confidence approvals

2 high-confidence denials

1 borderline case

Each explanation includes the top contributing features and their directional effect on the prediction.

Saved as:
xai_outputs/lime_explanation_case_1.html
xai_outputs/lime_explanation_case_2.html
xai_outputs/lime_explanation_case_3.html
xai_outputs/lime_explanation_case_4.html
xai_outputs/lime_explanation_case_5.html

A text summary is also provided in:
lime_text_outputs.txt

✅ 4. Strategic Plan: 3 Actionable Underwriting Recommendations

Based on SHAP global importance patterns and LIME local explanations, the project proposes three actionable strategies for underwriting teams:

1. Prioritize Transparency in High-Risk Decisions

Use LIME and SHAP local explanations to justify borderline or denied applications, ensuring regulatory-compliant decision records.

2. Monitor Key Risk Drivers Identified by SHAP

Features with consistently high SHAP contributions (e.g., delinquency history, DTI ratio) should be integrated into enhanced risk monitoring and customer segmentation strategies.

3. Implement Fairness Checks on Sensitive Attributes

Use SHAP dependence plots to detect whether income, employment status, or other socio-economic features introduce potential bias across demographic groups.

These recommendations are listed in:
strategic_underwriting_recommendations.txt
