## 📎 Live Demo

👉 Open in Colab: [[PEGAR LINK AQUÍ](https://colab.research.google.com/github/marlborito117-maker/conectatel-customer-analysis/blob/main/notebooks/conectatel_customer_analysis.ipynb)]


# 📊 ConectaTel Customer Analysis

## 🎯 Objective
This project analyzes customer behavior in a telecom company (ConectaTel) to identify usage patterns, segment users, and generate actionable business insights.

---

## 🧠 Project Overview
The analysis follows an end-to-end data workflow including data cleaning, exploratory data analysis (EDA), feature engineering, customer segmentation, and business recommendations.

---

## 📂 Datasets
- **users**: customer demographic and subscription data (age, city, plan, registration date)
- **usage**: user activity data (calls, messages, call duration)
- **plans**: available subscription plans

---

## 🧹 Data Cleaning
- Handled missing values and detected null proportions
- Identified and replaced sentinel values (e.g., `-999`, `?`)
- Converted invalid entries to `NaN`
- Corrected inconsistent date formats
- Removed future dates (e.g., year 2026)

---

## 📈 Exploratory Data Analysis (EDA)
- Analyzed distributions of:
  - Age
  - Number of messages
  - Number of calls
  - Call duration (minutes)
- Compared behavior across plan types (Basic vs Premium)
- Identified skewed distributions and usage patterns

---

## ⚠️ Outlier Analysis
- Used boxplots and IQR method
- Found outliers mainly in:
  - Messages
  - Calls
  - Call duration
- Decision:
  - Outliers were **kept**, as they represent real high-usage customers

---

## ⚙️ Feature Engineering
Created aggregated metrics per user:
- Total messages
- Total calls
- Total call minutes

---

## 👥 Customer Segmentation

### 🔹 By Usage
- **Low usage**: < 5 calls and < 5 messages  
- **Medium usage**: < 10 calls and < 10 messages  
- **High usage**: remaining users  

### 🔹 By Age
- **Young**: < 30  
- **Adult**: < 60  
- **Senior**: 60+  

---

## 📊 Key Insights

- Most users fall into the **medium usage segment**
- A smaller group of **high-usage users** represents high business value
- Call duration shows a **right-skewed distribution**, indicating heavy users
- Adult users dominate the customer base
- There is a clear opportunity for **upselling and targeted segmentation**

---

## 💡 Business Recommendations

- Increase revenue through **upselling strategies** targeting medium users
- Create optimized plans for **low-usage customers** to reduce churn
- Retain high-value customers with **premium benefits**
- Personalize offers based on **usage behavior and age segmentation**

---

## ▶️ How to Run

1. Open the notebook in Google Colab or Jupyter Notebook
2. Run all cells sequentially
3. Review outputs and visualizations

---

## 🔁 Reproducibility
The analysis is fully reproducible using the provided notebook and datasets.

---

## 🛠️ Tools Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## 📌 Author
**Eduardo Garcia**  
Aspiring Data Analyst | Telecom & Data Background
