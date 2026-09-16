# 📊 Churn Analysis & Customer Intelligence

An end-to-end **Customer Churn Analysis** project using **SQL and Python** to identify high-risk OTT subscribers and understand the key factors behind customer churn.

## 🎯 Project Objective

The goal of this project is to analyze customer, subscription, and support data to answer:

* **Who** is churning?
* **Why** are customers leaving?
* **When** are customers most likely to churn?
* Which customer segments have the highest churn risk?
* How do support escalations and contract types relate to churn?

## 🛠️ Tech Stack

* **SQL** – Data extraction and analysis
* **Python** – Data cleaning, feature engineering and EDA
* **Pandas & NumPy** – Data manipulation
* **Matplotlib & Seaborn** – Data visualization
* **MySQL / SQLite** – Database
* **Jupyter Notebook** – Analysis

## 🗂️ Dataset

The project uses a relational database named `customer_churn` containing three main tables:

### `db_customer`

* customerid
* name
* country
* state
* gender
* dob
* interests
* pincode

### `db_subscription`

* customerid
* subscription_start_date
* subscription_type
* renewal_date
* plan_type
* contract_type
* cancellation_date
* cancellation_reason
* monthly_charges
* cltv
* churn_score

### `db_support`

* customerid
* complaint_date
* escalations
* csat_score
* comment

The tables are joined using `customerid`.

## 🔄 Project Workflow

```text
SQL Database
     ↓
Data Extraction
     ↓
Data Cleaning
     ↓
Feature Engineering
     ↓
Exploratory Data Analysis
     ↓
Visualization
     ↓
Churn Insights
     ↓
Business Recommendations
```

## 🧹 Data Preparation

The analysis includes:

* Renaming columns for clarity
* Removing low-value/noisy columns
* Converting date columns to datetime
* Standardizing categorical values
* Handling missing country values
* Removing duplicate support records

## ⚙️ Feature Engineering

New features were created, including:

* `churn_flag`
* `age`
* `tenure_days`
* `complaint_count`
* `churn_risk`

These features were used to better understand customer behavior and identify high-risk subscribers.

## 📈 Key Results

| KPI                          |     Result |
| ---------------------------- | ---------: |
| Customers Analyzed           |         21 |
| Churn Rate                   |     28.57% |
| Retention Rate               |     71.43% |
| ARPU                         |     ₹18.85 |
| Escalation Rate              |     19.05% |
| Average Tenure               | 1,527 days |
| Revenue at Risk              |     ₹73.94 |
| Escalation–Churn Correlation |       0.77 |

## 🔍 Key Insights

### 1. Contract Type

Monthly subscribers had a **55.6% churn rate**, compared with **8.3% for annual subscribers**.

### 2. Plan Type

Basic-plan subscribers showed the highest churn rate at **60%**.

### 3. Support Escalations

Support escalations showed a **0.77 correlation with churn**, making them one of the strongest behavioral signals in the dataset.

### 4. Regional Churn

Karnataka and Meghalaya showed particularly high churn rates, although the underlying customer bases are small.

## 💡 Business Recommendations

* Investigate the reasons behind high churn in Karnataka and Meghalaya.
* Review Basic-plan pricing and customer experience.
* Encourage monthly customers to migrate to annual subscriptions.
* Prioritize high- and medium-risk customers based on churn risk, CLTV and complaint history.

## 📌 Skills Demonstrated

* SQL
* Python
* Data Cleaning
* Feature Engineering
* Exploratory Data Analysis
* Data Visualization
* KPI Analysis
* Customer Segmentation
* Churn Analysis
* Business Insights

## 👨‍💻 Author

**Kunal**
Data Analyst | SQL & Python Churn Analytics

---

⭐ If you found this project useful, feel free to explore the analysis and insights!
