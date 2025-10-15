Dashboard with Insights and Bi.  https://public.tableau.com/app/profile/jake.smith4051/viz/DafaultAnalysis/Story1?publish=yes


# Credit-and-Default-Risk-Analysis-
Diving into Reasons and Cautions for Default Rates and Providing Insights.  This projects shows skills in analytics stack (SQL, TABLEAU as well as PYTHON) 

# Credit Risk Analytics & Loan Default Prediction

### Overview
This project builds an **end-to-end Credit Risk Analytics pipeline**, combining:
- **SQL** for data extraction and preprocessing  
- **Python** for analysis, feature engineering, and predictive modeling  
- **Tableau** for business visualization and storytelling  

The goal is to assess **loan default probability** and identify **key drivers of credit risk**, enabling smarter lending decisions and improved risk management.

---

### Objective
To predict the likelihood of loan default based on borrower demographics, income, and credit history — and to visualize portfolio-level risk patterns for business decision-making.

---

### Tools & Technologies
- **SQL / SQLite** – Data extraction, joins, and aggregation  
- **Python (pandas, scikit-learn, matplotlib, seaborn)** – EDA and modeling  
- **Tableau** – Interactive dashboard for portfolio insights  
- **Jupyter Notebook** – Exploratory analysis and modeling environment  

---

### Project Structure
| Component | Description |
|------------|-------------|
| `credit_data.db` | SQLite database containing raw loan and customer data |
| `credit_queries.sql` | SQL script for extracting and cleaning the dataset |
| `Credit_Risk_Analysis.ipynb` | Python notebook for EDA, modeling, and evaluation |
| `Credit_Risk_Dashboard.twb` | Tableau dashboard for KPI visualization |
| `README.md` | Project overview and documentation |

---

### Analysis & Modeling Process

#### 1. **Data Extraction & Cleaning (SQL)**
- Joined customer, loan, and payment tables  
- Filtered active loans, removed missing IDs and outliers  
- Aggregated metrics: default rate by region, loan purpose, and employment type  

#### 2. **Exploratory Data Analysis (Python)**
- Investigated variable distributions and correlations  
- Visualized income vs. loan amount vs. default probability  
- Encoded categorical features and scaled numerical variables  

#### 3. **Predictive Modeling**
- **Baseline:** Logistic Regression (interpretable and simple)  
- **Enhanced:** Random Forest (captures non-linear patterns)  
- Addressed class imbalance using `class_weight='balanced'`  
- Evaluated models with recall, precision, and confusion matrix  

#### 4. **Key Findings**
- High default risk among low-income borrowers and self-employed applicants  
- Short credit history and high loan-to-income ratio = strong predictors of default  
- Certain loan purposes (e.g., personal, small business) carry higher risk  
- Regional variation shows distinct economic patterns in repayment behavior  

---

### 📊 Tableau Dashboard Highlights
- Portfolio-level KPIs: default rate, approval rate, average income  
- Risk segmentation by region, employment type, and loan purpose  
- Dynamic filters and drilldowns for interactive exploration  
- Intuitive color coding (green = low risk, red = high risk)  

**Dashboard Title Suggestion:**  
> “Credit Risk Overview — Loan Default Insights”

---

### Overall Business Impact
This project demonstrates how analytics can:
- Identify **high-risk borrowers** before approval  
- Support **data-driven lending strategies**  
- Visualize portfolio performance for **executive decision-making**  
- Improve **profitability and compliance** by aligning with risk policies  

---

###  Results Summary
| Metric | Logistic Regression | Random Forest |
|---------|---------------------|----------------|
| Accuracy | 0.78 | 0.84 |
| Recall (Default Class) | 0.62 | 0.71 |
| Precision | 0.68 | 0.75 |
| ROC-AUC | 0.82 | 0.89 |

> Random Forest improved recall and ROC-AUC, making it a stronger model for risk identification.  

---

### Economic Rationale
Rooted in **applied economics**, this project uses predictive analytics to balance **default risk** vs. **expected loan profit** — a real-world trade-off that credit institutions face daily.  

---

### Next Steps
1. Add **SHAP values** for model interpretability  
2. Include **profit-based optimization** (Expected Return = Revenue × (1 − Default Probability))  
3. Add **regional economic indicators** to enrich model features  
4. Deploy dashboard to Tableau Public for recruiter access  

---

### Author
**Jake Smith**  
MSc in Applied Economics | Data Analyst  
[jakesmith648@gmail.com] | [https://www.linkedin.com/in/jacob-smith-a46318153/]  

---

### Last Updated
October 2025
