# 📊 Customer Churn Analysis: Insights-Driven Retention Strategies

## 📌 Project Overview
This project analyzes a **Telco Customer dataset** to uncover drivers of **customer churn** (i.e., why customers leave the service).  
The focus is on **Exploratory Data Analysis (EDA)**, **visualization**, and **business insights**, without building machine learning models.  

The goal: **help businesses understand churn patterns and design data-driven retention strategies.**

---

## 🗂️ Dataset
- **Source:** Telco Customer Churn dataset (7,043 customers)
- **Target variable:** `Churn` (Yes/No)
- **Key features:** Demographics, contract type, payment method, services subscribed, tenure, charges.

---

## ⚙️ Steps in the Project
1. 📥 **Data Loading & Cleaning**  
   - Removed irrelevant identifiers (e.g., `customerID`).  
   - Handled missing values (`TotalCharges`).  

2. 🔍 **Exploratory Data Analysis (EDA)**  
   - Univariate analysis of numerical & categorical features.  
   - Bivariate analysis with respect to `Churn`.  
   - Correlation heatmap.  

3. 📊 **Visualizations**  
   - Churn distribution pie chart.  
   - Contract type vs churn.  
   - Tenure groups vs churn.  
   - MonthlyCharges distribution.  
   - Payment methods & services usage patterns.  

4. 🔧 **Feature Engineering**  
   - Created `AvgChargesPerMonth`.  
   - Derived `MultipleServices` (count of services subscribed).  
   - Tenure groups for lifecycle analysis.  

5. 📏 **Feature Scaling**  
   - Applied `StandardScaler` for numerical features (e.g., `tenure`, `MonthlyCharges`, `TotalCharges`).  

6. 💡 **Insights & Recommendations**  
   - Identified churn drivers (contract type, tenure, high charges, lack of support/security).  
   - Provided actionable recommendations for reducing churn.  

---

## 🔑 Key Insights
- **Contract type:** Month-to-month customers churn **42.7%**, vs **2.8%** for 2-year contracts.  
- **Tenure:** Most churn happens in the **first 12 months**.  
- **Pricing:** Higher `MonthlyCharges` strongly correlate with churn.  
- **Services:** Customers with **OnlineSecurity/TechSupport** churn much less.  
- **Payment method:** **Electronic check users** churn the most (**45.3%**).  
- **Demographics:** Senior citizens and customers without partners/dependents churn more.  

---

## 🧭 Recommendations
1. Convert **month-to-month customers** into long-term contracts via loyalty offers.  
2. Provide **early onboarding programs** during first 6–12 months.  
3. Reduce **price shock** for high-bill customers with bundles.  
4. Cross-sell **security & support services** to reduce churn risk.  
5. Encourage **auto-pay methods** (lower churn risk than electronic check).  
6. Build a **churn monitoring dashboard** for real-time insights.  

---

## 🔭 Future Work
- Build a **predictive churn model** (Logistic Regression, Random Forest, XGBoost).  
- Develop **customer segmentation** (clustering) for personalized retention.  
- Run **A/B testing** on retention strategies (e.g., contract conversion offers, service bundles).  
- Deploy results in a **dashboard (Power BI / Tableau)** for business stakeholders.  

---

## 📸 Sample Visualizations
*(Add screenshots from your notebook here – e.g., churn distribution pie chart, churn by contract, heatmap, etc.)*  

![Churn Distribution](churn_dist (1).png)  
![Churn by Contract](churn_bycont.png)  

---


## 🛠️ Tech Stack
- **Python**: pandas, numpy, matplotlib, seaborn, scikit-learn  
- **Jupyter Notebook** for analysis & visualization  
- _(Optional for future)_: Power BI / Tableau for dashboarding  

---

## 🙌 Acknowledgements
Dataset reference: Telco Customer Churn Dataset (Kaggle / IBM Sample Dataset).  
Special thanks to the open-source Python community for libraries that make data analysis powerful and accessible.  
