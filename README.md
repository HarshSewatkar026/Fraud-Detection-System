# 💳 Banking Fraud Detection System

## 📌 Project Overview  
This project focuses on building a Machine Learning model to detect fraudulent financial transactions. The goal is to improve fraud detection accuracy, minimize financial losses, and provide actionable business insights.

The solution covers the complete ML lifecycle — from data analysis to deployment.

---

## 🎯 Objectives  
- Detect fraudulent transactions with high accuracy  
- Reduce false negatives (missed fraud cases)  
- Analyze financial impact of fraud  
- Build a deployable real-time prediction system  

---

## 📊 Dataset Description  

The dataset contains simulated banking transactions with the following features:

| Feature | Description |
|--------|------------|
| step | Time step (1 step = 1 hour) |
| type | Transaction type (CASH-IN, CASH-OUT, DEBIT, PAYMENT, TRANSFER) |
| amount | Transaction amount |
| nameOrig | Sender account |
| oldbalanceOrg | Sender balance before transaction |
| newbalanceOrig | Sender balance after transaction |
| nameDest | Receiver account |
| oldbalanceDest | Receiver balance before transaction |
| newbalanceDest | Receiver balance after transaction |
| isFraud | Target variable (1 = Fraud, 0 = Legitimate) |

---

## 🔍 Project Workflow  

### 1. Data Exploration (EDA)
- Checked missing values and data distribution  
- Identified class imbalance  
- Visualized fraud patterns by transaction type and amount  

---

### 2. Feature Engineering  
- Created new features:
  - Balance difference (origin & destination)  
- Removed irrelevant columns (IDs)  
- Applied One-Hot Encoding  

---

### 3. Model Building  
Models implemented:
- Logistic Regression  
- Random Forest (Best Performing)  
- Gradient Boosting  

---

### 4. Model Evaluation  
Evaluation metrics used:
- Precision  
- Recall  
- F1-Score  
- ROC-AUC  

Focus was on Recall to minimize fraud loss.

---

### 5. Financial Impact Analysis  

Estimated financial loss using:

Expected Loss = False Negatives × Average Fraud Amount  

This helps quantify business risk due to undetected fraud.

---

### 6. Deployment  

- Model saved using `.pkl` file  
- Deployed using Streamlit  
- Built an interactive UI for real-time predictions  

---

### 7. Dashboard  

Created Power BI Dashboard including:
- Fraud overview  
- Financial impact  
- Model performance metrics  

---

## 🚀 How to Run the Project  

### Clone the repository
