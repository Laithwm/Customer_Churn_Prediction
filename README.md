# 📊 Customer Churn Prediction

Predicting whether a telecom customer will leave (churn) using **machine learning and exploratory data analysis**.

This project walks through a complete data science workflow — from cleaning and exploration to model building and evaluation — with an emphasis on interpretability and actionable business insights.

---

## 🧠 Project Summary

Telecom providers lose millions in recurring revenue each year due to customer churn.  
This project analyzes a Telco dataset to uncover the key behavioral, demographic, and service-related factors that drive customer retention.

The workflow focuses on:
- **Understanding churn patterns**
- **Building interpretable models**
- **Improving customer retention strategies**

---

## 📂 Repository Structure

```
Customer_Churn_Prediction/
│
├── 📁 Data
│   └── Telco-Customer-Churn.csv        # Dataset used for analysis
│
├── 📁 Notebook
│   └── customer_churn_analysis.ipynb   # Main notebook: EDA + model building
│
└── 📄 README.md                         # Project documentation
```

---

## ⚙️ Approach

### **1. Data Preprocessing**
- Handled missing values and categorical variables  
- Encoded non-numeric features (e.g., gender, contract type, payment method)  
- Normalized continuous variables like tenure and charges  

### **2. Exploratory Data Analysis (EDA)**
- Visualized churn distribution across key demographics  
- Identified trends by internet service, contract duration, and payment type  
- Found that:
  - **Month-to-month contracts** had the highest churn  
  - **Electronic check payments** were more common among churned customers  
  - Customers with **fiber optic internet** showed higher churn rates  

### **3. Model Development**
- Trained multiple models for comparison:
  - **Logistic Regression** (baseline)
  - **Decision Tree**
  - **Random Forest**
- Evaluated using:
  - Accuracy
  - Recall (sensitivity to churn)
  - Precision and F1-score

### **4. Evaluation**
- Random Forest achieved the best performance, balancing accuracy and recall.  
- Identified the most important features influencing churn:
  - `Contract`, `tenure`, `PaymentMethod`, and `InternetService`.

---

## 📈 Results

| Model | Accuracy | Key Strength |
|--------|-----------|--------------|
| Logistic Regression | ~80% | Simple, interpretable baseline |
| Decision Tree | ~83% | Captures nonlinear relationships |
| Random Forest | ~86% | Most robust and generalizable |

---

## 🧰 Tools & Libraries

| Category | Tools |
|-----------|-------|
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Environment | Jupyter Notebook |

---

## 💡 Key Insights
- **Contract type** is the strongest indicator of churn likelihood.  
- Customers using **electronic check payments** churn significantly more.  
- **Tenure** and **monthly charges** are major retention levers.  

These insights can guide business teams to target at-risk customers through contract incentives or payment method migration.

---

## 🚀 Future Work
- Introduce **XGBoost** for improved predictive performance  
- Use **SHAP values** for explainable feature impact  
- Build a **Streamlit dashboard** for live churn risk scoring  

---

## 👤 Author

**Laith Waqas Mohammed**  
_Data Scientist | Visual Storyteller | Analyst_  
📍 Dublin, Ireland   
💼 [LinkedIn](https://www.linkedin.com/in/laithwm)

---
