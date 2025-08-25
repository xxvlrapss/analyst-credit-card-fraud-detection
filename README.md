# 💳 Credit Card Fraud Detection  

![Python](https://img.shields.io/badge/Python-3.9-blue?logo=python)  
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple?logo=pandas)  
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-green?logo=plotly)  
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)  
![Scikit-Learn](https://img.shields.io/badge/ScikitLearn-ML-yellow?logo=scikitlearn)  
![Tableau](https://img.shields.io/badge/Tableau-Dashboard-blue?logo=tableau)  

---

## ✨ Project Summary  
This project analyzes **284,807 credit card transactions** to detect fraudulent activity.  
Fraudulent transactions represent only **0.172% of the data**, creating a significant **class imbalance problem**.  
The goal is to identify **patterns in fraud**, build detection models, and provide **business recommendations** to improve fraud prevention strategies.  

---

## 📖 Context  
- **Industry Challenge**: Credit card companies must detect fraud quickly to avoid losses and protect customer trust.  
- **Dataset**: 284,807 transactions collected over two days.  
- **Fraud Cases**: Only 492 transactions are labeled as fraud (0.172%).  
- **Problem**: Extreme imbalance makes traditional accuracy metrics misleading; specialized methods are needed.  

---

## 📂 Dataset  
- **Source**: [Kaggle – Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)  
- **Shape**: 284,807 transactions × 31 columns  
- **Key Features**:  
  - `Time`: seconds elapsed since first transaction.  
  - `Amount`: transaction amount.  
  - `V1–V28`: anonymized PCA components.  
  - `Class`: target variable (0 = Non-Fraud, 1 = Fraud).  

---

## 🔎 Insights  

### 📉 Current Fraud Rate  
- Fraud occurs in **<0.2% of all transactions**.  
- Traditional accuracy is misleading → better to use **Precision-Recall AUC or F1-Score**.  

### ⏰ Temporal Fraud Patterns  
- Fraud is **not evenly distributed** but concentrated at specific times.  
- Indicates potential for **time-based monitoring** to catch fraud in real-time.  

### 📊 Feature Distribution Differences  
- PCA features such as **V4, V11, and V14** show clear distribution differences between fraud and non-fraud.  
- These features are strong candidates for **feature selection** in machine learning models.  

---

## ✅ Recommendations  

### ⏱️ Vulnerable Time Monitoring  
- Increase monitoring sensitivity during periods when fraud is most common.  

### 🛠️ Feature Engineering  
- Focus model development on discriminative features (e.g., V4, V11, V14) to improve fraud detection accuracy.  

### ⚖️ Imbalanced Data Handling  
- Apply **SMOTE, undersampling, or cost-sensitive learning** to address class imbalance.  

### 🚨 Real-Time Alert System  
- Integrate time-based fraud patterns and transaction amount thresholds into a **real-time alert system** for faster investigation.  

---

## 📊 Visualizations  

- **Interactive Dashboard (Tableau)**:  
  👉 [Credit Card Fraud Detection Dashboard](https://public.tableau.com/app/profile/dimas.prayoga7117/viz/Visualisasi_Analysis_CreditCardFraudDetectionMLGULB/Dashboard1)  
