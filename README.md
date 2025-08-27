# Personal Loan Propensity Modeling

## 📌 Context
A National Bank in the US with a growing customer base needed insights on customer purchasing loads. The majority of these customers are **liability customers** (depositors) with varying sizes of deposits. The number of customers who are also borrowers (**asset customers**) is quite small, and the bank is interested in expanding this base rapidly to bring in more loan business — and in the process, earn more through interest on loans.  

In particular, management wants to explore ways of converting its liability customers into **personal loan customers** (while retaining them as depositors).

A campaign run last year for liability customers showed a **conversion rate of over 9%**, encouraging the retail marketing department to design campaigns with better target marketing to further increase the success ratio.

As a **Data Scientist** at AllLife Bank, your task is to build a model that helps the marketing department identify potential customers with a higher probability of purchasing a loan.

---

## 🎯 Objective
- Predict whether a liability customer will purchase a personal loan.  
- Identify the most significant customer attributes driving purchases.  
- Highlight the customer segments to target for higher conversion.

---

## 🗂 Data Dictionary

| Feature              | Description |
|----------------------|-------------|
| `ID`                 | Customer ID |
| `Age`                | Customer’s age (years) |
| `Experience`         | Years of professional experience |
| `Income`             | Annual income (in thousand USD) |
| `ZIP Code`           | Home address ZIP code |
| `Family`             | Family size |
| `CCAvg`              | Average monthly credit card spending (in thousand USD) |
| `Education`          | Education level: 1 = Undergrad, 2 = Graduate, 3 = Advanced/Professional |
| `Mortgage`           | Value of house mortgage (in thousand USD) |
| `Personal_Loan`      | Loan acceptance in the last campaign (0 = No, 1 = Yes) |
| `Securities_Account` | Has securities account? (0 = No, 1 = Yes) |
| `CD_Account`         | Has certificate of deposit (CD) account? (0 = No, 1 = Yes) |
| `Online`             | Uses internet banking? (0 = No, 1 = Yes) |
| `CreditCard`         | Uses a credit card issued by another bank? (0 = No, 1 = Yes) |

---

## 🔬 Approach & Methodology

1. **Data Understanding & Cleaning**  
   - Verified data completeness and consistency.  
   - Handled missing or anomalous values (e.g., negative experience years).  
   - Checked for class imbalance in the target variable (`Personal_Loan`).

2. **Exploratory Data Analysis (EDA)**  
   - Visualized distributions of numerical variables (Age, Income, CCAvg).  
   - Analyzed correlations between features and personal loan acceptance.  
   - Profiled customers by education level, income bracket, and credit usage.

3. **Feature Engineering**  
   - Created derived features (e.g., income‑to‑mortgage ratio, spending‑to‑income ratio).  
   - Encoded categorical variables where necessary.  
   - Normalized/standardized numerical variables for model compatibility.

4. **Model Selection & Training**  
   - Compared baseline models: Logistic Regression, Decision Trees, and Gradient Boosting.  
   - Applied **HyperParameter Optimization (HPO)** to tune model performance.  
   - Used **cross‑validation** to ensure robustness.

5. **Model Evaluation**  
   - Evaluated using Accuracy, Precision, Recall, F1‑score, and ROC‑AUC.  
   - Assessed top predictive features to provide business‑ready insights.

6. **Business Impact Translation**  
   - Translated predictive outputs into actionable customer segments for targeted marketing.  
   - Estimated potential lift over the previous 9% conversion rate through focused campaigns.

---

## 📈 Expected Outcomes
- Higher marketing ROI through **data‑driven targeting**.  
- Improved **conversion rates** for personal loan campaigns.  
- Clear understanding of **key drivers** influencing loan uptake.

---

## 🚀 Next Steps
- Deploy the model as an API endpoint for integration into CRM systems.  
- Automate periodic retraining using updated customer data.  
- Conduct A/B testing of targeted campaigns to validate uplift predictions.
