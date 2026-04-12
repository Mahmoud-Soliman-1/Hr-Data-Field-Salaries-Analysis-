# 📊 HR Salary Analysis & Prediction

## 📌 Project Overview
This project analyzes global data-related job salaries from an HR perspective and builds a machine learning model to predict expected salaries based on candidate attributes.

The goal is to help HR professionals:
- Understand salary trends in the data field
- Compare roles, experience levels, and company factors
- Estimate fair salary ranges for candidates

---

## 📁 Dataset Description

The dataset contains information about data professionals, including:

- `work_year`
- `experience_level`
- `employment_type`
- `job_title`
- `salary`
- `salary_currency`
- `salary_in_usd`
- `employee_residence`
- `remote_ratio`
- `company_location`
- `company_size`

---

## 🧹 Data Preparation

Steps performed using Python:

- Merged multiple data sources
- Removed duplicates
- Handled missing values
- Standardized salaries using `salary_in_usd`
- Created new features:
  - `job_category` (grouped job titles into major categories)
  - `same_country` (whether employee and company are in the same country)

---

## 📊 Data Analysis (Power BI Dashboard)

A full interactive dashboard was created to analyze the market from an HR perspective.

### 🔹 Page 1: Market Overview
- Median Salary
- Headcount
- Remote Work Percentage
- Salary Trend Over Time
- Salary by Job Function
- Job Distribution
- Remote Distribution

### 🔹 Page 2: Experience & Company Analysis
- Salary by Experience Level
- Salary by Company Size
- Combined impact of experience and company size

### 🔹 Page 3: Location & Remote Analysis
- Salary by Country
- Remote vs Onsite distribution by location
- Cross-country employment insights

---

## 🤖 Machine Learning Model

### 🎯 Objective
Predict salary based on candidate and job attributes.

### 📌 Target
- `salary_in_usd` (log-transformed)

### 📌 Features
- Experience Level
- Employment Type
- Company Size
- Job Category
- Employee Residence
- Company Location
- Remote Ratio
- Same Country Indicator

---

## ⚙️ Feature Engineering

- Applied **Label Encoding** for ordinal features (experience level)
- Applied **One-Hot Encoding** for categorical features
- Reduced country dimensionality using:
  - Top countries + "Other"
- Created `same_country` feature

---

## 📈 Model Approach

- Used **Random Forest Regressor**
- Applied **log transformation** on salary to handle skewness
- Predictions are converted back using exponential transformation

---

## 📊 Evaluation Metrics

- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R² Score

---

## 🛠️ Tools & Technologies

- Python (Pandas, NumPy, Scikit-learn)
- Power BI
- Data Cleaning & EDA
- Machine Learning

---

## 📌 Key Insights

- Salary strongly depends on experience level and job category
- Company size and location influence compensation
- Remote roles show different salary patterns depending on geography

---

## 📬 Contact

Mahmoud Soliman  
Data Analyst  
mahmoudsoliman1503@gmail.com
---

⭐ If you found this project useful, feel free to star the repository!
