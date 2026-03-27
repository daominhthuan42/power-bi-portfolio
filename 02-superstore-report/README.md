# 🏬 Superstore Sales Analytics 🔍

**Notebook:** `superstore-sales-analysis.ipynb`  
**Dashboard Export:** `super-store.pbix`  
**Author:** Đào Minh Thuấn  
**Project Type:** Python (EDA, Customer Analytics, Business Intelligence)

---

## 🧭 Project Overview

This project analyzes a **retail Superstore dataset** at the transaction level to uncover insights into **sales performance, profitability, and customer behavior**.

The analysis combines **descriptive analytics and customer-centric modeling**, including segmentation, retention analysis, and value-based evaluation.

Key analytical techniques include:

* **Exploratory Data Analysis (EDA)**
* **RFM Segmentation**
* **Cohort Analysis (Retention & Churn)**
* **Pareto (80/20) Analysis**
* **Quarter-over-Quarter (QoQ) Growth Analysis**
* **Customer Segmentation using K-Means**

The goal is to generate **actionable insights** that support decision-making in **sales strategy, customer retention, and profitability optimization**.

---

## 🎯 Objectives

* Analyze sales and profit distribution across products and regions.
* Segment customers based on purchasing behavior.
* Evaluate customer retention and churn patterns.
* Identify high-value customers and revenue drivers.
* Support business decisions with data-driven insights.

---

## 📂 Dataset Information

* **Size:** 9,994 transaction records
* **Features:** 20 columns
* **Granularity:** Order line-item level
* **Target:** Unsupervised (no predefined labels)

---

## 🔑 Key Features

### Order & Time

* `OrderID`, `OrderDate`, `ShipDate`, `ShipMode`

### Customer

* `CustomerID`, `CustomerName`, `Segment`

### Geography

* `Country`, `Region`, `State`, `City`, `PostalCode`

### Product

* `ProductID`, `Category`, `Sub-Category`, `ProductName`

### Business Metrics

* `Sales`, `Quantity`, `Discount`, `Profit`

---

## 🧪 Data Quality Assessment

* **Missing Values:** None detected
* **Duplicates:** 1 duplicated record (~0.01%) → negligible impact
* **Outliers:** Present in `Sales`, `Quantity`, `Discount`, `Profit`

👉 These outliers are **business-driven** (bulk orders, high discounts), not data errors.

Dataset is suitable for **analysis without heavy preprocessing**.

---

## 📊 Analysis & Key Outputs

### 🔎 Sales Overview

![Overview](https://iili.io/qtP4yJ9.png)

* High-level KPIs: **Sales, Profit, Orders**
* Breakdown by **Region, Category, and Time**
* Identifies top-performing segments and trends

---

### 🧠 RFM Customer Segmentation

![RFM Analysis](https://iili.io/qtPXViG.png)

* Segments customers based on:

  * **Recency (R)**
  * **Frequency (F)**
  * **Monetary (M)**
* Identifies key groups:

  * **Champions**
  * **Loyal Customers**
  * **At Risk**
  * **Hibernating**
* Supports targeted **retention and marketing strategies**

---

### 🔄 Cohort Analysis (Retention)

![Cohort Analysis](https://iili.io/qtiHNbR.png)

![Retention Rate](https://iili.io/qtiH4Js.png)

* Tracks customer retention based on **first purchase month**
* Measures **retention rate over time (Month Offset)**
* Highlights **early churn behavior**
* Enables evaluation of customer lifecycle performance

---

### 📉 QoQ (Quarter-over-Quarter) Analysis

![QoQ Analysis](https://iili.io/qtihMNI.png)

* Analyzes **quarterly trends** in:

  * Sales
  * Profit
  * Order volume
* Calculates **QoQ growth rates**
* Identifies:

  * Growth periods
  * Seasonal patterns
  * Performance fluctuations

---

### 💰 Customer Value Analysis (CLV Proxy)

![CLV Analysis](https://iili.io/qtiS5oQ.png)

* Estimates **customer value using aggregated revenue** (proxy for CLV)
* Segments customers into:

  * Low-value
  * Medium-value
  * High-value
* Highlights **top revenue-contributing customers**

⚠️ Note:
This is a **descriptive CLV proxy**, not a predictive CLV model.

---

### 🤖 Customer Segmentation (K-Means)

![KMean](https://iili.io/qtsRgLB.png)

* Applies **K-Means clustering** on customer features
* Groups customers based on:

  * Purchase behavior
  * Spending patterns
* Supports **unsupervised segmentation beyond RFM**

---

### 👤 Customer Profiling

![Profiling](https://iili.io/qtsRe5b.png)

![Profiling2](https://iili.io/qtsRSzQ.png)

* Profiles customer segments based on:

  * Demographics (Region, Segment)
  * Purchase patterns
* Provides business-friendly interpretation of clusters

---

## 🧠 Business Insights

* Sales and profit distribution are **highly skewed** → a small group of customers drives most revenue.
* **High-value segments (Champions, Loyal)** contribute disproportionately → prioritize retention.
* Heavy discounts often **reduce profitability**, especially in certain categories.
* Customer retention shows **early drop-off** → onboarding and early engagement are critical.
* Regional differences indicate **opportunities for localized strategy optimization**.

---

## 🚀 Future Improvements

* Build **predictive models** for Sales or Profit.
* Develop **true CLV prediction models** (e.g., BG/NBD, Gamma-Gamma).
* Optimize **K-Means clustering** (feature scaling, silhouette score).
* Integrate **interactive dashboards** (Power BI / Plotly Dash).
* Implement **customer churn prediction models**.

---

## 👤 Author

**Name:** Đào Minh Thuấn
**GitHub:** [https://github.com/daominhthuan42](https://github.com/daominhthuan42)
