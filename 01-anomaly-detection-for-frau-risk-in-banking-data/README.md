# 🏦 Anomaly Detection for Fraud Risk in Banking Data 🛡️

**Notebook:** `anomaly-detection-for-frau-risk-in-banking-data.ipynb`  
**Dashboard Export:** `anomaly-detection-for-frau-risk-in-banking-data.pbix`  
**Author:** Đào Minh Thuấn  
**Project Type:** Power BI + Python  

---

## 🧭 Project Overview

Fraud detection is a critical challenge in banking, where real-world datasets are often **unlabeled** due to privacy constraints and limited accessibility.

This project analyzes a **synthetic bank transaction dataset** and applies **unsupervised learning techniques** to identify potentially fraudulent activities.

Dataset original:
[https://www.kaggle.com/datasets/valakhorasani/bank-transaction-dataset-for-fraud-detection](https://www.kaggle.com/datasets/valakhorasani/bank-transaction-dataset-for-fraud-detection)

Dataset (cleaned & synthetic version):
[https://www.kaggle.com/datasets/thuandao/bank-transactions-dataset-for-fraud-detection](https://www.kaggle.com/datasets/thuandao/bank-transactions-dataset-for-fraud-detection)

### 🎯 Objectives

* Explore transaction behavior and detect anomalies.
* Apply **unsupervised models** (Clustering + Isolation Forest).
* Analyze customer value using **RFM and CLV models**.
* Provide actionable insights for **fraud risk management and business optimization**.

### 🧠 Approach

This project combines:

* **Behavioral segmentation** (RFM Analysis)
* **Customer value modeling** (CLV)
* **Unsupervised anomaly detection** (Isolation Forest, Clustering)
* **Time-based analysis** (Cohort, QoQ)
* **Data visualization** using Power BI

---

## 📂 Dataset Information

* **Size:** 50,000 transactions
* **Features:** 15 columns
* **Target:** Unsupervised (no fraud labels)

### 🔑 Key Features

**Transaction Data**

* `TransactionID`, `TransactionAmount`, `TransactionDate`, `TransactionDuration`

**Account Information**

* `AccountID`, `AccountBalance`

**Customer Attributes**

* `CustomerAge`, `CustomerOccupation`

**Channel & Device**

* `Channel`, `DeviceID`, `IP Address`, `Location`, `MerchantID`

**Security**

* `LoginAttempts`

---

## 📊 Dashboard Overview

### 🔎 Overview

![Overview](https://iili.io/qte84HX.png)

* Provides a high-level summary of key metrics: **total transaction amount, total transactions, total customers, and average transaction value**.
* Displays **monthly trends**, **merchant performance**, **channel distribution**, and **geographic insights**.
* Helps identify **top-performing segments and operational patterns**.

---

### 👥 RFM Analysis

![RFM](https://iili.io/qteZnDB.png)

* Segments customers based on **Recency, Frequency, and Monetary (RFM)** metrics.
* Uses **Treemap visualization** to classify groups such as *Champions, Loyal, At Risk, Hibernating*.
* Includes **Pareto analysis** to evaluate revenue contribution.
* Supports targeted strategies for **retention and engagement**.

---

### 📅 Cohort Analysis

![Cohort](https://iili.io/qtkHyDG.png)

* Tracks **customer retention over time** based on first transaction month.
* Highlights **early churn patterns** and retention decay.
* Enables evaluation of **customer lifecycle performance** across cohorts.

---

### 📊 QoQ Analysis

![QoQ Analysis](https://iili.io/qtkBfwP.png)

* Focuses on **Quarter-over-Quarter (QoQ) performance trends**.
* Tracks key KPIs: **transaction amount, revenue, and customer count** across quarters.
* Includes **QoQ growth rates** to identify acceleration or slowdown in business performance.
* Helps assess **short-term business momentum** and detect seasonal patterns or anomalies.

---

### 💰 CLV Analysis

![CLV Analysis](https://iili.io/qtk1sLu.png)

* Focuses on **Customer Lifetime Value (CLV)** to measure long-term customer profitability.
* Shows **CLV distribution** and segments customers into **Low, Medium, High-value tiers**.
* Highlights **top customers by CLV** for prioritization.
* Supports strategies for **customer retention, personalization, and revenue maximization**.

---

### 🚨 Anomalies Analysis

![Anomalies Analysis](https://iili.io/qtvtGQ2.png)

* Visualizes fraud detection results using **Isolation Forest**.
* Displays separation between **normal vs. anomalous transactions** using PCA (2D projection).
* Shows **anomaly score distribution** and threshold.
* Includes detailed table of **flagged suspicious transactions**.

* Visualizes fraud detection results using **KMean and Local Outlier Factor**.

![KMean Analysis](https://iili.io/qtL5e07.png)

![LOF Analysis](https://iili.io/qtL5OfS.png)

---

### 🔬 Advanced Analysis

![Advanced Analysis](https://iili.io/qtvgDUQ.png)

* Compares **normal vs. potential fraudulent transactions** across multiple dimensions:

  * Transaction amount
  * Channel & transaction type
  * Customer demographics
  * Account balance & duration
* Identifies behavioral differences that may indicate fraud patterns.
* Geographic map highlights **fraud concentration areas**.

---

### 📈 Anomaly Trends

![Anomaly Trends](https://iili.io/qtvwW9s.png)

* Tracks **monthly trends of transaction behavior** for normal vs. anomalous groups.
* Reveals that:

  * At the **transaction level**, anomalies often involve irregular patterns (e.g., duration, frequency).
  * At the **aggregated level**, anomalies may show **higher average transaction values due to periodic spikes**.
* Supports monitoring of **fraud pattern evolution over time**.

---

## 💡 Key Insights & Recommendations

### 🔍 Fraud Insights

**Fraud Behavior Summary (Isolation Forest Results)**

* Fraudulent transactions often exhibit **unusual patterns in duration and frequency** rather than just extreme values.
* Higher anomaly likelihood is observed in **Credit transactions** and **Branch/Online channels**.
* Slightly higher occurrence among **older customers**, with minimal occupation-based differences.
* Accounts associated with anomalies tend to have **lower balances**.
* Fraud patterns are **not strongly location-dependent**.
* Fraud signals are **volatile over time**, indicating periodic spikes rather than stable trends.

---

### 🏦 Business Recommendations

* Implement **real-time anomaly monitoring systems** using Isolation Forest.
* Combine **rule-based detection** with machine learning models for robustness.
* Prioritize **manual review for high-value customers with anomalies**.
* Design **targeted retention campaigns** for cohorts with early churn signals.
* Continuously monitor **QoQ performance and anomaly trends** to detect emerging risks.

---

## 👤 Author

* **Name:** Đào Minh Thuấn
* **GitHub:** [https://github.com/daominhthuan42](https://github.com/daominhthuan42)
