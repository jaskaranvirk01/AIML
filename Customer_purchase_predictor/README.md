# Customer Purchase Prediction (ShopSmart E‑commerce)

## 📌 Project Overview

This project focuses on predicting whether a website visitor will complete a purchase on an e‑commerce platform using their browsing behavior. By leveraging machine learning, the goal is to help businesses identify high‑intent users and optimize marketing, UX, and conversion strategies.

The project uses **exploratory data analysis (EDA)** and a **Decision Tree–based classification pipeline** to model customer purchase behavior.

---

## 🎯 Problem Statement

E‑commerce platforms receive thousands of visitors daily, but only a small percentage convert into paying customers. Without predictive insights, marketing efforts and user engagement strategies remain inefficient.

**Objective:**
Build a supervised machine learning model that predicts whether a user session will result in a purchase (`Revenue = True / False`) based on browsing behavior.

---

## 📊 Dataset Description

The dataset represents individual user sessions from an e‑commerce website. Each session is unique to avoid bias from repeat users.

**Target Variable**

* `Revenue` (Boolean → converted to 0/1)

**Feature Categories**

* **Behavioral Metrics**: Page values, bounce rates, exit rates
* **Page Interaction**: Administrative, Informational, Product‑related pages and durations
* **Temporal & Contextual**: SpecialDay, Month, VisitorType, Weekend

---

## 🔍 Exploratory Data Analysis (EDA)

EDA was performed to compare users who **purchased** vs **did not purchase**.

Key visual analyses include:

* Purchase vs non‑purchase distribution (pie chart)
* Average page value comparison
* Product‑related page visits & time spent
* Bounce rate & exit rate comparison
* Administrative and informational page behavior
* Impact of `SpecialDay` on purchasing decisions

**Insights:**

* Purchasing users show significantly higher `PageValues`
* Buyers interact more with product‑related pages
* Lower bounce and exit rates correlate with conversions

---

## 🧠 Machine Learning Approach

### Model Used

* **Decision Tree Classifier**

### Why Decision Tree?

* Interpretable rules
* Handles non‑linear relationships well
* Works effectively with mixed feature types

---

## ⚙️ Data Preprocessing

A robust preprocessing pipeline was created using `ColumnTransformer`:

* **Numerical Features** → StandardScaler
* **Categorical Features** → OneHotEncoder (`handle_unknown='ignore'`)

This ensures consistent and leak‑free preprocessing during training and evaluation.

---

## 🏗️ Pipeline Architecture

```
Preprocessing (Scaling + Encoding)
        ↓
Decision Tree Classifier
```

The pipeline guarantees that all transformations are applied identically during training, testing, and cross‑validation.

---

## 📈 Model Evaluation

The model was evaluated on a stratified 80/20 train‑test split using:

* Accuracy
* Precision
* Recall
* F1‑Score

This ensures balanced performance evaluation, especially for imbalanced classes.

---

## 🔎 Hyperparameter Tuning

`GridSearchCV` with 5‑fold cross‑validation was used to optimize:

* `max_depth`
* `min_samples_leaf`

**Scoring Metric:** F1‑Score (balances precision & recall)

This step significantly improves model generalization and robustness.

---

## 🛠️ Technologies Used

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit‑learn
* Jupyter Notebook

---

## 🚀 Key Takeaways

* User engagement metrics are strong predictors of conversion
* Decision Trees provide both performance and interpretability
* Pipelines & cross‑validation are critical for production‑ready ML

---

## 📌 Future Improvements

* Try ensemble models (Random Forest, XGBoost)
* Handle class imbalance using SMOTE
* Deploy the model using Flask/FastAPI
* Build a real‑time prediction dashboard

---

## 👤 Author

**JASS Virk**
Aspiring Data Scientist | Machine Learning Enthusiast
