📊 Employee Attrition Prediction using Machine Learning
📌 Project Overview

Employee attrition is a major concern for organizations as it impacts productivity, cost, and workforce planning.
This project focuses on predicting employee attrition (whether an employee will leave the company or not) using Machine Learning classification algorithms.

The project uses Logistic Regression and Random Forest Classifier to analyze HR data and identify key factors contributing to employee attrition.

🎯 Objectives

Analyze employee data to understand attrition patterns

Preprocess and clean HR dataset

Build and evaluate multiple ML models

Handle class imbalance effectively

Identify important features affecting attrition

Visualize insights using data visualization techniques

🗂 Dataset Information

Dataset Name: WA_Fn-UseC_-HR-Employee-Attrition.csv

Target Variable: Attrition

Yes → 1 (Employee left)

No → 0 (Employee stayed)

Dataset contains employee demographics, job roles, salary details, work experience, and satisfaction metrics.

🛠 Tools & Technologies Used

Programming Language: Python

Libraries:

NumPy

Pandas

Matplotlib

Seaborn

Scikit-learn

🔄 Project Workflow
1️⃣ Data Loading & Exploration

Loaded dataset using Pandas

Checked dataset shape, data types, missing values

Performed basic exploratory data analysis (EDA)

Analyzed class imbalance in the target variable

2️⃣ Data Cleaning & Feature Selection

Dropped irrelevant columns:

EmployeeCount

EmployeeNumber

Over18

StandardHours

Converted Attrition into numerical format (0/1)

3️⃣ Data Preprocessing

Separated categorical and numerical features

Applied One-Hot Encoding for categorical variables

Performed Feature Scaling using StandardScaler

Ensured clean and consistent target labels

4️⃣ Train-Test Split

Split data into:

80% Training

20% Testing

Used stratified sampling to handle class imbalance

🤖 Machine Learning Models Used
🔹 Logistic Regression

Implemented baseline Logistic Regression model

Evaluated using:

Accuracy

Confusion Matrix

Precision, Recall, F1-score

Used class_weight="balanced" to improve minority class prediction

🔹 Random Forest Classifier

Built ensemble-based Random Forest model

Tuned hyperparameters:

n_estimators

max_depth

Used GridSearchCV with F1-score as evaluation metric

Extracted Top 10 important features influencing attrition

📈 Model Evaluation Metrics

Accuracy Score

Confusion Matrix

Classification Report

Precision

Recall

F1-score

Special focus was given to Recall and F1-score since attrition prediction is a class-imbalanced problem.

📊 Data Visualization & Insights

The following visualizations were created to understand employee behavior:

Attrition Count Plot

Age vs Attrition (Boxplot)

Monthly Income Distribution by Attrition

Pairplot of key numerical features

These visuals help identify trends such as:

Age groups with higher attrition

Income distribution differences

Relationship between tenure and attrition

🔑 Key Insights

Attrition is influenced by factors such as:

Monthly Income

Age

Years at Company

Job Role

Random Forest performed better than Logistic Regression

Class imbalance significantly affects predictions, handled using:

Stratified sampling

Balanced class weights

F1-score optimization
