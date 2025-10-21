<<<<<<< HEAD
# Customer_Churn_Prediction
=======
# Customer Churn Production on Telco's dataset

Predicting whether a telecom customer will leave (churn) using machine-learning models.  
This project demonstrates an end-to-end data-science workflow — data cleaning, exploratory analysis, feature engineering, model training, and evaluation.

---

## The Dataset 

- **Source:** [Kaggle – Telco Customer Churn](https://www.kaggle.com/blastchar/telco-customer-churn)  
- **Rows:** 7 043 customers  
- **Target:** `Churn` (Yes / No)  
- **Features:** Customer demographics, contract type, payment method, tenure, monthly & total charges, and more.  

---

## Data Cleaning And Preprocessing 

- Loaded the dataset with **Pandas** and reviewed structure using `.info()` and `.describe()`.  
- Converted the `TotalCharges` column to numeric (`errors="coerce"`) to fix non-numeric entries.  
- Checked for missing values and handled them appropriately.  
- Encoded categorical variables using one-hot encoding / label encoding for ML compatibility.  
- Split data into **train** and **test** sets.  

---

## Exploratory Data Analysis (EDA)  

- **Tenure Distribution:** Most customers have short tenure; longer-tenure customers churn less.  
- **Monthly Charges:** Higher monthly charges correlate with a greater likelihood of churn.  
- **Total Charges:** Reflects customer lifetime value; high total charges usually mean loyal customers.  
- **Contract Type & Churn:** Month-to-month contracts show the highest churn rates.  
- **Correlation Heatmap:** Revealed positive correlation between `MonthlyCharges` and churn, negative correlation with `tenure`.  

Visualizations created using **Matplotlib** and **Seaborn**.  

---

## Modeling Approach  

Built and evaluated four supervised-learning models:  
1. **Logistic Regression**  
2. **Decision Tree Classifier**  
3. **Random Forest Classifier**  
4. **XGBoost Classifier**  

Metrics used: Accuracy, Precision, Recall, F1-Score, Confusion Matrix.  

---

## Results  

| Model | Accuracy | Precision (Churn) | Recall (Churn) | F1 |
|:------|:----------|:------------------|:---------------|:--|
| Logistic Regression | 0.80 | 0.65 | 0.50 | 0.56 |
| Decision Tree | 0.73 | 0.49 | 0.52 | 0.51 |
| Random Forest | 0.79 | 0.64 | 0.51 | 0.57 |
| **XGBoost** | **0.81** | **0.67** | **0.53** | **0.59** |

**XGBoost** delivered the best performance (≈ 81 % accuracy).  

---

## Feature Importance & Insights  

- **Contract Type**, **Tenure**, and **Monthly Charges** are top predictors of churn.  
- **Month-to-Month contracts** and **high monthly charges** strongly increase churn risk.  
- **Automatic payments** and **long-term contracts** lower churn probability.  

---

## How To Run 
```bash
git clone https://github.com/Laithwm/Customer_Churn_Prediction.git
cd Customer_Churn_Prediction
pip install -r requirements.txt
jupyter notebook notebooks/customer_churn_analysis.ipynb
```





>>>>>>> 9aeff8e0eb7c163deb468b35eeb860f30520e73b
