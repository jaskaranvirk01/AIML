# CreditWise – Loan Approval Prediction System 💳📊

## 📌 Project Overview
**CreditWise** is a machine learning project that predicts whether a loan application will be **approved or rejected** based on an applicant’s financial and personal details.

The project focuses on selecting the **most reliable model** using **precision** as the key evaluation metric to minimize risky loan approvals.

---

## 🧠 Problem Statement
Financial institutions face challenges in accurately approving loans. Wrong approvals can cause losses, while wrong rejections reduce customer trust.

This project aims to:
- Analyze loan applicant data
- Build predictive machine learning models
- Compare multiple algorithms
- Select the best-performing model based on precision

---

## 📂 Dataset Description
The dataset includes:
- Applicant demographic information  
- Financial and credit-related attributes  
- Loan status (Target variable)

Data is cleaned and preprocessed to ensure high-quality model training.

---

## 🔄 Project Workflow

### 1️⃣ Libraries Used
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

### 2️⃣ Data Preprocessing
- Loaded dataset using Pandas
- Handled missing values
- Cleaned and formatted data
- Converted data types where necessary

---

### 3️⃣ Exploratory Data Analysis (EDA)
- Visualized numerical feature distributions
- Analyzed categorical variables
- Identified trends, patterns, and outliers

---

### 4️⃣ Encoding
- Converted categorical variables into numerical form
- Prepared data for machine learning models

---

### 5️⃣ Correlation Analysis
- Created correlation heatmap
- Identified important relationships between features
- Reduced multicollinearity

---

### 6️⃣ Feature Engineering
- Selected relevant features
- Removed unnecessary columns
- Improved model efficiency

---

### 7️⃣ Train-Test Split & Scaling
- Split data into training and testing sets
- Applied feature scaling where required

---

## 🤖 Models Implemented
The following supervised learning models were trained and evaluated:

1. Naive Bayes  
2. Logistic Regression  
3. K-Nearest Neighbors (KNN)  

---

## 📊 Evaluation Metric
**Precision** was used as the primary evaluation metric because:
- False positives (approving risky loans) are costly
- Precision ensures reliable loan approvals

---

## 🏆 Model Performance (Based on Precision)
1. 🥇 **Naive Bayes** – Best Model  
2. 🥈 Logistic Regression  
3. 🥉 K-Nearest Neighbors (KNN)  

**Naive Bayes** achieved the highest precision and was selected as the final model.

---

## 📈 Conclusion
- Proper preprocessing and feature engineering improved results
- Naive Bayes outperformed other models
- Precision-based evaluation is effective for financial risk prediction

---
## 👤 Author

**JASS Virk**
Aspiring Data Scientist | Machine Learning Enthusiast