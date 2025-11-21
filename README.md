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

