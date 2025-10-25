# loan-risk-analysis-CRISPDM
Machine Learning project for FinTech Innovations: a profit-optimized, interpretable loan approval model using Logistic Regression and Random Forest. Built end-to-end following the CRISP-DM framework, featuring data preprocessing pipelines, EDA visuals, cost-sensitive evaluation, and threshold tuning to maximize business impact.
###  Project Overview
This project applies machine learning to modernize FinTech Innovations’ loan approval process.  
The goal is to replace manual, inconsistent reviews with a **data-driven, interpretable, and profit-optimized decision system**.

---

###  Objectives
- Develop a predictive model to automate or support loan approval decisions.  
- Minimize costly false approvals (defaults) while identifying overlooked creditworthy applicants.  
- Ensure regulatory transparency and fairness across applicant segments.  
- Deliver an end-to-end pipeline aligned with the **CRISP-DM** methodology.

---

###  Approach (CRISP-DM Framework)
1. **Business Understanding** — Define the costs of false approvals vs. false denials.  
2. **Data Understanding** — Perform EDA on 20,000 historical loan records with financial & behavioral indicators.  
3. **Data Preparation** — Build preprocessing pipelines using `ColumnTransformer` for numerical and categorical features.  
4. **Modeling** — Train and tune Logistic Regression and Random Forest classifiers with GridSearchCV.  
5. **Evaluation** — Assess models using ROC-AUC, Balanced Accuracy, and a **custom Expected Profit metric**.  
6. **Deployment Recommendation** — Select the profit-maximizing Logistic Regression model for implementation.

---

###  Key Results
| Model | Best Threshold | Expected Profit | Key Traits |
|--------|----------------|----------------|-------------|
| **Logistic Regression** | 0.95 | **≈ \$5.08M** | High interpretability, conservative, regulatory-friendly |
| **Random Forest** | 0.50 | ≈ \$3.09M | Captures more approvals but higher defaults |

**Top Predictors:** Credit Score, Debt-to-Income Ratio, Payment History, Interest Rate, Job Tenure.  

---

###  Tech Stack
- **Language:** Python  
- **Libraries:** pandas, scikit-learn, matplotlib, seaborn, numpy  
- **Framework:** CRISP-DM (Cross-Industry Standard Process for Data Mining)  
- **Environment:** Jupyter Notebook  
