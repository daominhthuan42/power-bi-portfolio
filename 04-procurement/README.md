# 🏦 Anomaly Detection for Fraud Risk in Banking Data 🛡️

**Notebook:** `bank_transaction.ipynb`  
**Dashboard Export:** `bank_transaction.pbix`  
**Author:** Đào Minh Thuấn  
**Project Type:** Power BI + Python  

---

## 🧭 Project Overview

Fraud detection remains a critical challenge in banking, where real-world datasets are often unlabeled due to privacy constraints and limited accessibility.

In this project, I analyze a bank transaction dataset and apply unsupervised learning techniques to detect potentially fraudulent activities without relying on predefined labels.

Dataset original: [Banking_Transactional_Dataset](https://docs.google.com/spreadsheets/d/1MZ3B7n9GjrZfMJlFwUUP_dBuWglUFv1r/edit?gid=210684686#gid=210684686)

### 🎯 Objectives

* Analyze transaction behavior and identify anomalies
* Apply **unsupervised models** (Isolation Forest & LOF)
* Segment customers using **RFM analysis**
* Evaluate customer value through **CLV**
* Deliver actionable insights for **fraud risk management and business optimization**

### 🧠 Approach

This project combines:

* **Behavioral segmentation** (RFM Analysis)
* **Customer value modeling** (CLV)
* **Unsupervised anomaly detection** (Isolation Forest, LOF)
* **Time-based analysis** (Cohort, QoQ)
* **Data visualization** using Power BI

---

## 📂 Dataset Information

* **Size:** 20,000 transactions
* **Features:** 19 columns
* **Target:** Unsupervised (no fraud labels)

### 🔑 Key Features

| Column             | Description                                                                  |
| ------------------ | ---------------------------------------------------------------------------- |
| TransactionID      | Unique identifier for each transaction                                       |
| CustomerID         | Unique identifier for each customer                                          |
| TransactionDate    | Date when the transaction occurred                                           |
| TransactionType    | Type of transaction (e.g., Deposit, Withdrawal, Transfer, Card Payment, Fee) |
| Amount             | Monetary value of the transaction                                            |
| ProductCategory    | Financial product category associated with the transaction                   |
| ProductSubcategory | More detailed classification within the product category                     |
| BranchCity         | City where the branch or transaction took place                              |
| BranchLat          | Latitude of the branch                                                       |
| BranchLong         | Longitude of the branch                                                      |
| Channel            | Channel used for the transaction (e.g., Branch, ATM, Mobile)                 |
| Currency           | Currency used in the transaction                                             |
| CreditCardFees     | Fees incurred from credit card usage                                         |
| InsuranceFees      | Fees related to insurance                                                    |
| LatePaymentAmount  | Penalty amount due to late payment                                           |
| CustomerScore      | Credit score or internal customer rating                                     |
| MonthlyIncome      | Customer’s monthly income                                                    |
| CustomerSegment    | Customer segment based on income                                             |
| RecommendedOffer   | Recommended product or offer for the customer                                |

---

## 📊 Dashboard Overview

### 🔎 Overview

![Overview](https://iili.io/BO1J1VV.png)

* Provides a high-level overview of key metrics: **total transaction amount, total transactions, average monthly income, and average transaction value**.
* Displays **monthly transaction trends**, highlighting fluctuations and year-over-year growth.
* Breaks down performance by **customer segments, transaction types, and channels** (Branch, ATM, Mobile, Online).
* Visualizes **geographic distribution of transactions** and identifies **top-performing cities**.
* Helps uncover **spending patterns, customer behavior, and potential anomalies across segments and locations**.

---

### 👥 Customer Insight

![Customer Insight](https://iili.io/BO1AoP9.png)

* Provides an overview of **segment performance across years**, highlighting differences between middle, high, and low-income customer groups.
* Analyzes **product usage by customer segment**, showing how different segments interact with financial products (loans, credit cards, savings, etc.).
* Visualizes the relationship between **credit score and customer behavior**, helping identify patterns and potential risk signals.
* Enables comparison of **customer value distribution and engagement across segments**.
* Supports detection of **behavioral anomalies and segment-specific trends** for deeper analysis.

---

### 💰 Revenue & Behavior

![Revenue & Behavior](https://iili.io/BO1MnVa.png)

* Provides a high-level overview of **total amount, total transactions, total fees, and average fee per transaction**.
* Breaks down **fee components** (late payment, insurance, credit card) to highlight main revenue drivers.
* Compares **transaction volume vs. fee revenue** across transaction types to evaluate efficiency and profitability.
* Analyzes **offer performance by revenue**, identifying top-performing financial products and campaigns.
* Evaluates **channel performance** (ATM, Branch, Mobile, Online) across customers, transactions, amount, and fees.
* Helps uncover **revenue patterns, fee structures, and optimization opportunities across channels and products**.

---

### 👥 RFM Analysis

![RFM Analysis](https://iili.io/BO1kW41.png)

* Provides an overview of **customer base and RFM metrics**: Recency, Frequency, and Monetary value.
* Segments customers into groups such as **Champions, Loyal, At Risk, Potential Loyalists, and Hibernating**.
* Visualizes **customer distribution across segments**, helping identify high-value and at-risk groups.
* Applies **Pareto analysis (80/20 rule)** to highlight key segments contributing the most revenue.
* Analyzes detailed **RFM scores at customer level**, enabling deeper behavioral insights.
* Supports identification of **customer retention opportunities, re-engagement strategies, and revenue concentration risks**.

---

### 📅 Cohort Analysis

![Retenion Customer](https://iili.io/BO1pXxp.png)

![Retenion Rate](https://iili.io/BO1phWN.png)

* Visualizes **customer retention by cohort**, tracking behavior after the first transaction month.
* Displays **retention rate over time**, highlighting how customer engagement declines across months.
* Provides both **percentage-based retention** and **absolute customer counts** for deeper analysis.
* Enables comparison across cohorts to identify **strong vs. weak retention periods**.
* Helps uncover **customer lifecycle patterns, churn behavior, and long-term engagement trends**.
* Supports identification of **retention improvement opportunities and early drop-off risks**.

---

### 📊 QoQ Analysis

![QoQ Analysis](https://iili.io/BOExIGn.png)

* Visualizes **quarter-over-quarter (QoQ) growth in transaction amount** across customer segments.
* Compares performance between **high, middle, and low-income segments** over time.
* Highlights **growth trends and fluctuations**, including periods of acceleration and decline.
* Enables tracking of **segment-level contribution to overall revenue performance**.
* Helps identify **seasonality patterns, segment volatility, and potential downturn signals**.
* Supports analysis of **revenue dynamics and strategic focus across customer segments**.

---

### 💎 CLV Analysis

![CLV Analysis](https://iili.io/BOExRaf.png)

* Provides an overview of **customer value metrics**, including average transaction value, purchase frequency, customer lifetime, and customer lifetime value (CLV).
* Breaks down **CLV by customer segment**, highlighting differences between low, middle, and high-income groups.
* Tracks **revenue per customer over time**, showing monthly trends and growth patterns.
* Analyzes **customer-level performance**, including income, transaction behavior, and lifetime contribution.
* Helps identify **high-value customers and key revenue drivers** across segments.
* Supports optimization of **customer retention, targeting strategies, and long-term value maximization**.

---

### 🌲 Isolation Forest

![Anomalies Analysis](https://iili.io/BOEPjJp.png)

![Profiling Customer](https://iili.io/BOEPXgR.png)

* Applies **unsupervised anomaly detection (Isolation Forest)** to identify potential fraudulent transactions.
* Compares **behavioral patterns between normal and anomalous transactions** across multiple features (amount, fees, income, etc.).
* Analyzes distribution across **transaction types, channels, products, and locations** to detect abnormal concentrations.
* Visualizes anomalies using **PCA (2D projection)** to highlight separation between normal and suspicious transactions.
* Evaluates **anomaly score distribution** to define thresholds and distinguish fraud vs. normal behavior.
* Helps uncover **hidden fraud patterns, unusual customer behavior, and high-risk transaction profiles**.

---

### 🔬 Local Outlier Factor

![Anomalies Analysis](https://iili.io/BOGFkTF.png)

![Profiling Customer](https://iili.io/BOGFOp1.png)

* Applies **Local Outlier Factor (LOF)** to detect anomalies based on **local density deviations** in the data.
* Compares **normal vs. anomalous behavior** across multiple features (amount, fees, income, etc.).
* Analyzes distributions across **transaction types, channels, products, and locations** to identify abnormal patterns.
* Visualizes anomalies using **PCA (2D projection)** to highlight clusters of suspicious transactions.
* Evaluates **LOF score distribution**, where higher scores indicate stronger anomaly likelihood.
* Helps uncover **localized anomalies and subtle behavioral deviations** that may not be captured by global models.

---

## 💡 Key Insights & Recommendations

### 🔍 Fraud Insights

**Fraud Behavior Summary (Isolation Forest Results)**

* Fraudulent transactions exhibit **higher amounts and significantly higher fees**, indicating strong anomaly signals.
* Anomalies are **highly concentrated in Loan Payment transactions**, suggesting a **clear and isolated fraud pattern**.
* Higher fraud occurrence is observed in **Loan and Credit Card products**, indicating **strong product-specific risk concentration**.
* Fraud is **evenly distributed across channels and locations**, showing **no channel or geographic dependency**.
* Customers associated with anomalies have **slightly lower income**, but this remains a **weak signal**.
* Fraud appears across all segments, with slightly higher presence in **middle and low-income groups**.
* Fraud patterns are **highly distinct and extreme**, making them easier to detect using global anomaly detection methods.

**Fraud Behavior Summary (Local Outlier Factor Results)**

* Fraudulent transactions show **higher amounts and elevated fees**, but with more overlap compared to global models.
* Anomalies are **more broadly distributed across transaction types**, with a moderate peak in **Loan Payment**.
* Fraud is **evenly distributed across channels and locations**, indicating **no channel or geographic dependency**.
* Higher anomaly presence is observed in **Loan and Credit Card products**, suggesting **moderate product-related risk signals**.
* Customers associated with anomalies tend to have **lower income levels**, indicating **financial stress as a stronger signal**.
* Slightly higher occurrence in **low and middle-income segments**, with weaker signals in high-income groups.
* Fraud patterns are **more subtle and locally driven**, capturing **behavioral deviations rather than extreme outliers**.

---

## 💡 Key Takeaways

* Fraud patterns are driven by a mix of **extreme anomalies** and **subtle behavioral deviations**
* **Loan-related transactions and fee patterns** are the strongest fraud indicators
* Fraud is **not dependent on geography or channel**
* **Customer income and segmentation** provide additional risk signals
* Different models capture **different dimensions of fraud behavior**

## 👤 Author

* **Name:** Đào Minh Thuấn
* **GitHub:** [https://github.com/daominhthuan42](https://github.com/daominhthuan42)
