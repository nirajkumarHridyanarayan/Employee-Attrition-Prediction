# 📊 Employee Attrition Prediction using Machine Learning

## 📌 Project Overview
Employee attrition is a major concern for organizations as it directly impacts productivity, operational costs, and workforce planning.  
This project focuses on predicting employee attrition (whether an employee will leave the organization or not) using Machine Learning classification algorithms.

The project leverages Logistic Regression and Random Forest Classifier to analyze HR data and identify key factors contributing to employee attrition.

---

## 🎯 Project Objectives
- Analyze employee data to understand attrition patterns  
- Preprocess and clean the HR dataset  
- Build and evaluate multiple Machine Learning models  
- Handle class imbalance effectively  
- Identify important features affecting attrition  
- Visualize insights using data visualization techniques  

---

## 🗂 Dataset Information
- **Dataset Name:** `WA_Fn-UseC_-HR-Employee-Attrition.csv`  
- **Target Variable:** `Attrition`
  - `Yes` → **1** (Employee Left)
  - `No` → **0** (Employee Stayed)
- The dataset includes:
  - Employee demographics  
  - Job roles and departments  
  - Salary and compensation details  
  - Work experience and tenure  
  - Job satisfaction and performance metrics  

---

## 🛠 Tools & Technologies Used
- **Programming Language:** Python  
- **Libraries:**
  - NumPy  
  - Pandas  
  - Matplotlib  
  - Seaborn  
  - Scikit-learn  

---

## 🔄 Project Workflow

### 1️⃣ Data Loading & Exploration
- Loaded the dataset using Pandas  
- Checked dataset shape, data types, and missing values  
- Performed Exploratory Data Analysis (EDA)  
- Analyzed class imbalance in the target variable  

---

### 2️⃣ Data Cleaning & Feature Selection
- Dropped irrelevant columns:
  - `EmployeeCount`
  - `EmployeeNumber`
  - `Over18`
  - `StandardHours`
- Converted `Attrition` into numerical format (0 / 1)

---

### 3️⃣ Data Preprocessing
- Separated categorical and numerical features  
- Applied One-Hot Encoding for categorical variables  
- Performed Feature Scaling using `StandardScaler`  
- Ensured clean and consistent target labels  

---

### 4️⃣ Train–Test Split
- Split the dataset into:
  - **80% Training Data**
  - **20% Testing Data**
- Used stratified sampling to handle class imbalance  

---

## 🤖 Machine Learning Models Used

### 🔹 Logistic Regression
- Implemented baseline Logistic Regression model  
- Evaluated using:
  - Accuracy  
  - Confusion Matrix  
  - Precision, Recall, and F1-score  
- Used `class_weight="balanced"` to improve minority class prediction  

---

### 🔹 Random Forest Classifier
- Built an ensemble-based Random Forest model  
- Tuned hyperparameters:
  - `n_estimators`
  - `max_depth`
- Used GridSearchCV with F1-score as the evaluation metric  
- Extracted Top 10 important features influencing attrition  

---

## 📈 Model Evaluation Metrics
- Accuracy Score  
- Confusion Matrix  
- Classification Report:
  - Precision  
  - Recall  
  - F1-score  

📌 Special focus was given to Recall and F1-score since employee attrition is a class-imbalanced problem.

---

## 📊 Data Visualization & Insights
The following visualizations were created to understand employee behavior:

- Attrition Count Plot  
- Age vs Attrition (Boxplot)  
- Monthly Income Distribution by Attrition  
- Pairplot of key numerical features  

These visualizations helped identify:
- Age groups with higher attrition  
- Income distribution differences  
- Relationship between tenure and attrition  

---

## 🔑 Key Insights
- Attrition is influenced by:
  - Monthly Income  
  - Age  
  - Years at Company  
  - Job Role  
- Random Forest outperformed Logistic Regression  
- Class imbalance was handled using:
  - Stratified sampling  
  - Balanced class weights  
  - F1-score optimization  

---

## 🧠 Conclusion
This project demonstrates an end-to-end Machine Learning pipeline for predicting employee attrition, covering:
- Data preprocessing  
- Model training and hyperparameter tuning  
- Performance evaluation  
- Insightful visualizations  

This project is well-suited for showcasing skills required for:
- Data Analyst  
- Data Scientist  
- Machine Learning Engineer  

---
