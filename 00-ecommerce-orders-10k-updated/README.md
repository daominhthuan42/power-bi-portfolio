# 🛒 E-commerce Orders 🔍

**Notebook:** `ecommerce-orders-10k-updated.ipynb` <br>
**Dashboard Export:** `ecommerce-orders-10k-updated.pbix` <br>
**Author:** Đào Minh Thuấn <br>
**Project Type:** Power BI + Python

## 🧭 Project Overview

* The dataset contains **transaction-level information**: order_id, user_id, product_id, category, price, quantity, total_price, order_date, country, and customer_segment.
* It enables analysis of **shopping behaviors** based on product categories, spending levels, and customer segments.
* Key variables such as **total_price**, **category**, **customer_segment**, and **country** support revenue analysis, RFM segmentation, and customer profiling.
* The dataset is suitable for **Customer Segmentation**.

Dataset original: [E-commerce Orders Dataset](https://github.com/elizabethwanjiku703/Youtube/blob/main/Tutorial%2010/ecommerce_orders_10k_updated.csv)

**Goal:**

* Data analytics (segmentation, cohort analysis).
* Customer value modeling (RFM, CLV).
* Data visualization with Power BI.

## 📂 Dataset Information

**Size:** 10000 transactions, 10 features.
**Target:** ***Unsupervised*** (no fraud labels provided).

### 🔑 Key Features

* **Order:** `order_id`, `price`, `qty`, `total_price`, `order_date`.
* **Account:** `user_id`, `country`.
* **Product:** `product_id`, `category`.

## 🎯 Objectives

### Overview

![Overview](https://iili.io/fnOpcZP.png)

* This is an **e-commerce orders dashboard**, summarizing key metrics such as total sales, quantity sold, number of orders, and average order value, with year-over-year comparison and filters by country and year.
* It visualizes **sales distribution by category, month, customer segment, quarter, and country**, including a map and Top-5 countries table.
* The dashboard helps identify **high-performing categories, regions, and customer segments**, supporting decisions on marketing, inventory planning, and overall sales strategy.

### xTD Performance

![xTD Performance](https://iili.io/fneKiDG.png)

* This page presents the **x-to-Date (MTD / QTD / YTD) e-commerce orders performance**, including key metrics such as **Sales, Quantity Sold, Orders, and Average Order Value**, all benchmarked against the prior year.
* It provides insights into **monthly sales trends vs last year**, **Top 20 customers by xTD sales**, **country-level performance**, and **customer-segment contribution** in both sales and AOV.
* It supports monitoring **xTD growth** and evaluating the effectiveness of **customer segments and key markets (countries)** to guide targeting, retention, and marketing decisions.

### RFM

![RFM](https://iili.io/fneTLkQ.png)

* This page presents the **customer analysis based on the RFM model** (Recency – Frequency – Monetary) along with average RFM metrics.
* Customers are segmented (Champions, Loyal, At Risk, Hibernating, etc.) using a **Treemap**, and their revenue contribution is evaluated through a **Pareto Analysis**.
* It helps identify **high-value customers**, those needing attention, and those at risk of churn to support targeted strategies.

### Cohort

![Cohort](https://iili.io/fne7EiP.png)

* This page shows a **Cohort Retention Analysis**, tracking the number and percentage of customers retained each month after their first transaction.
* It highlights **early churn patterns**, the gradual decline in retention over time, and differences across cohorts.
* It helps evaluate **customer retention performance** and identify segments that require improvement or additional engagement.

### CLV & QoQ

![CLV & QoQ](https://iili.io/fnecaOG.png)

* This page provides a **quarterly analysis** of transaction amount, revenue, and customer count, including **Quarter-over-Quarter (QoQ) growth trends**.
* It shows the **distribution of Customer Lifetime Value (CLV)** and the breakdown of **CLV segments** (Low, Medium, High value).
* Highlights the **top customers by CLV**, helping identify the most valuable long-term contributors.
