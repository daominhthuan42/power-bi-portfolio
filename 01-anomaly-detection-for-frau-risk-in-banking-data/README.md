# 🏦 Anomaly Detection for Fraud Risk in Banking Data 🛡️

**Notebook:** `Bank_Transactions.ipynb` <br>
**Dashboard Export:** `final_project.pbix` <br>
**Author:** Đào Minh Thuấn <br>
**Project Type:** Power BI + Python

## 🧭 Project Overview

Fraud detection is a critical challenge in banking, but real datasets are often **unlabeled** due to privacy and data scarcity.
This project analyzes a **synthetic bank transaction dataset** and applies **unsupervised anomaly detection & clustering** to identify potentially fraudulent transactions.

Dataset original: [Bank Transaction Dataset for Fraud Detection (Kaggle)](https://www.kaggle.com/datasets/valakhorasani/bank-transaction-dataset-for-fraud-detection)

Dataset clean (fake data): [Bank Transaction Dataset for Fraud Detection — Synthetic Data Generated with ChatGPT](https://github.com/daominhthuan42/datapot-data-analytics-bootcamp/blob/main/01_PL300-149/final-project/bank_transactions_data_2_augmented_clean_2.csv)

**Goal:**

* Explore transaction patterns and anomalies.
* Apply unsupervised models (Clustering + Isolation Forest) to detect suspicious activities.
* Provide insights for **fraud risk management**.

It combines:

* Data analytics (segmentation, cohort analysis).
* Customer value modeling (RFM, CLV).
* Fraud detection using anomaly analysis.
* Data visualization with Power BI.

## 📂 Dataset Information

**Size:** 50000 transactions, 15 features.
**Target:** ***Unsupervised*** (no fraud labels provided).

### 🔑 Key Features

* **Transaction:** `TransactionID`, `TransactionAmount`, `TransactionDate`, `TransactionDuration`.
* **Account:** `AccountID`, `AccountBalance`.
* **Customer Info:** `CustomerAge`, `CustomerOccupation`.
* **Channel & Devices:** `Channel`, `DeviceID`, `IP Address`, `Location`, `MerchantID`.
* **Security:** `LoginAttempts`.

## 🎯 Objectives

### Overview

![Overview](https://iili.io/fJxfmep.png)

* This is a **banking transaction overview dashboard**, showing key metrics such as total amount, total transactions, total customers, and average transaction value.
* It provides insights into **monthly trends, merchant performance, city distribution, transaction channels, and transaction types**.
* It helps identify **high-contribution locations, merchants, and channels**, supporting monitoring and business decision-making.

### xTD Performance

![xTD Performance](https://iili.io/fJxoKnS.png)

* This page presents the **x-to-Date (with x: MTD, YTD and QTD) transaction performance**, including key metrics such as Amount, Transactions, Average Transaction Value, and Average Customer Value compared to last year.
* It provides insights into **monthly trends**, **top-contributing customers**, **high-performing devices**, and **city-level growth**.
* It supports monitoring **xTD growth** and evaluating the effectiveness of customers, devices, and transaction channels.

### RFM

![RFM](https://iili.io/fJxurFI.png)

* This page presents the **customer analysis based on the RFM model** (Recency – Frequency – Monetary) along with average RFM metrics.
* Customers are segmented (Champions, Loyal, At Risk, Hibernating, etc.) using a **Treemap**, and their revenue contribution is evaluated through a **Pareto Analysis**.
* It helps identify **high-value customers**, those needing attention, and those at risk of churn to support targeted strategies.

### Cohort

![Cohort](https://iili.io/fJx553N.png)

* This page shows a **Cohort Retention Analysis**, tracking the number and percentage of customers retained each month after their first transaction.
* It highlights **early churn patterns**, the gradual decline in retention over time, and differences across cohorts.
* It helps evaluate **customer retention performance** and identify segments that require improvement or additional engagement.

### CLV & QoQ

![CLV & QoQ](https://iili.io/fJxYXp9.png)

* This page provides a **quarterly analysis** of transaction amount, revenue, and customer count, including **Quarter-over-Quarter (QoQ) growth trends**.
* It shows the **distribution of Customer Lifetime Value (CLV)** and the breakdown of **CLV segments** (Low, Medium, High value).
* Highlights the **top customers by CLV**, helping identify the most valuable long-term contributors.

### Anomalies Analysis

![Anomalies Analysis](https://iili.io/fJxcpXn.png)

* This page visualizes **fraud detection results** using the Isolation Forest model, showing the separation between **normal transactions and potential frauds** on a PCA 2D plot.
* The anomaly score distribution highlights the **threshold** and distinguishes the **fraud zone vs. normal zone**.
* A detailed table lists **flagged suspicious transactions**, including customer info, transaction details, and segment classification.

### Advanced Analysis

![Advanced Analysis](https://iili.io/fJx1kJ4.png)

* This page analyzes **fraud patterns** by comparing normal vs. potential fraud transactions across multiple dimensions.
* It examines differences in **transaction amount, channel, transaction type, customer age, occupation, account balance, and duration**.
* The geographic map highlights **where potential frauds are concentrated**.

### Anomaly Trends

![Anomaly Trends](https://iili.io/fJxGktS.png)

* This page shows the **monthly trend of average transaction amount** for normal vs. potential fraud transactions.
* It highlights a clear difference, with **potential frauds consistently having higher transaction values** than normal transactions.
* Helps monitor how the anomaly pattern changes across months.

## 💡 Key Insights & Recommendations

### 🔍 Fraud Insights

**Fraud Behavior Summary (Isolation Forest Results)**

* **Fraud tends to involve smaller amounts but longer transaction duration.**
* **Fraud occurs more frequently in Credit transactions and in Branch/Online channels.**
* **Fraud is more common among older customers, with no strong occupation differences, though Retired is slightly higher.**
* **Fraudulent accounts generally have lower balances than normal accounts.**
* **Regional differences are minimal, with no clear separation.**
* **Monthly trends are highly volatile, indicating periodic fraud spikes rather than steady behavior.**

### 🏦 Business Recommendations

* Implement **real-time monitoring rules** for repeated-pattern transactions.
* Combine rule-based checks with **Isolation Forest** for more robust detection.
* High-value customers with anomalies should trigger **priority manual review**.
* Introduce targeted **retention campaigns** for cohorts with early churn.
