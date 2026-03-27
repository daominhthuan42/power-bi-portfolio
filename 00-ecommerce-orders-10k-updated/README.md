# 🛒 E-commerce Orders Analytics 🔍

**Notebook:** `ecommerce-orders-10k-updated.ipynb`
**Dashboard:** `ecommerce-orders-10k-updated.pbix`
**Author:** Đào Minh Thuấn
**Project Type:** Data Analytics (Python + Power BI)

---

## 🧭 Project Overview

This project analyzes an e-commerce transaction dataset to uncover insights into customer behavior, revenue performance, and long-term customer value.

The dataset contains **transaction-level data**, including:

* Orders: `order_id`, `price`, `quantity`, `total_price`, `order_date`
* Customers: `user_id`, `country`, `customer_segment`
* Products: `product_id`, `category`

**total_price (GMV)** represents the total revenue per transaction.

The project supports:

* Revenue analysis
* Customer segmentation
* Retention and cohort analysis
* Customer lifetime value modeling

**Dataset:**
[E-commerce Orders Dataset](https://github.com/elizabethwanjiku703/Youtube/blob/main/Tutorial%2010/ecommerce_orders_10k_updated.csv)

---

## 📂 Dataset Information

* **Size:** 10,000 transactions
* **Features:** 10 columns
* **Type:** Unsupervised analysis (no labels provided)

---

## 🎯 Project Scope

* Customer segmentation (RFM)
* Cohort and retention analysis
* Customer Lifetime Value (CLV)
* Sales and growth performance analytics
* Time series analysis

---

## ⚙️ Tech Stack

* **Python:** data preprocessing, feature engineering
* **Power BI:** data modeling & dashboard visualization
* **DAX:** KPI calculations and business metrics

---

## 🧱 Data Model

* Star schema design:

  * **Fact table:** Orders (transactions)
  * **Dimension tables:** Customers, Products, Date

---

## 📊 Dashboard Pages

### 1. Overview

![Overview](https://iili.io/qtOOSHb.png)

* Provides a high-level view of **total revenue, orders, quantity, and AOV** with YoY comparison.
* Visualizes sales distribution by **category, country, segment, and time**.
* Supports identification of top-performing regions and product categories.

---

### 2. RFM Analysis

![RFM](https://iili.io/qLgqd0X.png)

* Segments customers using the **RFM model (Recency, Frequency, Monetary)**.
* Groups include **Champions, Loyal, At Risk, Hibernating**, etc.
* Includes **Pareto analysis** to evaluate revenue contribution.
* Helps prioritize retention and re-engagement strategies.

---

### 3. Cohort Analysis

![Cohort](https://iili.io/qLgAR6v.png)
![Retention Rate](https://iili.io/qLg1wSs.png)

* Tracks **customer retention over time** based on first purchase month.
* Highlights **churn patterns and retention decay**.
* Enables evaluation of long-term customer engagement.

---

### 4. CLV Analysis

![CLV](https://iili.io/qtOZ2Bn.png)

* Analyzes **Customer Lifetime Value (CLV)** along with:

  * Average Order Value (AOV)
  * Purchase Frequency
* Identifies **high-value customers** and revenue drivers.
* Supports strategies for **retention, upselling, and customer growth**.

---

### 5. QoQ Growth Analysis

![QoQ](https://iili.io/qte9pWl.png)

* Visualizes **quarter-over-quarter (QoQ) sales/quantity/orders trends** by category.
* Highlights **growth patterns, seasonality, and volatility**.
* Helps identify **high-growth and declining categories**.

---

### 6. Time Series Analysis

![Timeseries](https://iili.io/qL4TQ72.png)

* Tracks **daily revenue (GMV)** with moving averages:

  * 7-day, 14-day, 30-day
* Reduces noise to reveal **underlying trends and anomalies**.
* Supports **short-term monitoring and forecasting decisions**.

---

## 👤 Author

* **Name:** Đào Minh Thuấn
* **GitHub:** [https://github.com/daominhthuan42](https://github.com/daominhthuan42)

---

## ✅ Summary

This project transforms raw transactional data into actionable insights by combining **customer analytics, revenue modeling, and interactive dashboards**, enabling a shift from **transaction-based reporting to customer-centric decision-making**.
