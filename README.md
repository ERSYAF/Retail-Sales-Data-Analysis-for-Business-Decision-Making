# Retail-Sales-Data-Analysis-for-Business-Decision-Making
## 📌 Project Description

This project focuses on analyzing retail sales transaction data to support **business decision making** using a data-driven approach.

The dataset used in this project is the **Online Retail Dataset** from the UCI Machine Learning Repository / Kaggle. The dataset contains transaction records from a UK-based online retail company.

Dataset Source:
[Online Retail Dataset - Kaggle](https://www.kaggle.com/datasets/fareselgohary003/online-retail-transactions-uci)

---

# 📖 Business Background

A UK-based online retail company wants to improve sales performance and business decision making by utilizing historical transaction data.

Through retail sales analysis, the company aims to understand:

* Customer purchasing behavior
* Product performance
* Revenue contribution
* Sales trends
* Customer segmentation

The analysis is expected to support more effective and data-driven business strategies.

---

# 🎯 Business Problems

This project aims to answer several business questions:

* What are the best-selling products?
* Which countries contribute the highest revenue?
* How do sales trends change over time?
* Who are the high-value customers?
* How can customer segmentation improve marketing strategy?

---

# 🎯 Project Objectives

The objectives of this project are:

* Generate business insights from retail transaction data
* Understand sales patterns and customer behavior
* Support data-driven decision making
* Identify high-performing products and valuable customers
* Perform customer segmentation using RFM Analysis
* Build interactive business intelligence dashboards

---

# 🛠️ Technologies Used

| Technology            | Purpose                         |
| --------------------- | ------------------------------- |
| Python                | Data analysis                   |
| Pandas                | Data manipulation               |
| NumPy                 | Numerical analysis              |
| Matplotlib            | Data visualization              |
| Seaborn               | Statistical visualization       |
| Google Colab          | Development environment         |
| PostgreSQL / Supabase | Database integration            |
| Metabase              | Business intelligence dashboard |

---

# 📂 Dataset Information

## Dataset Features

| Feature     | Description           |
| ----------- | --------------------- |
| InvoiceNo   | Unique invoice number |
| StockCode   | Product identifier    |
| Description | Product description   |
| Quantity    | Purchased quantity    |
| InvoiceDate | Transaction date      |
| UnitPrice   | Price per item        |
| CustomerID  | Customer identifier   |
| Country     | Customer country      |

---

# 🔍 Initial Dataset Overview

## Raw Dataset Information

| Information   | Value   |
| ------------- | ------- |
| Total Rows    | 541,909 |
| Total Columns | 8       |

---

# ⚠️ Data Quality Findings

Several data quality issues were identified during preprocessing and validation.

## Missing Values

| Column      | Missing Values |
| ----------- | -------------- |
| CustomerID  | 135,080        |
| Description | 1,454          |

---

## Invalid Data

| Validation      | Total  |
| --------------- | ------ |
| Quantity ≤ 0    | 10,624 |
| UnitPrice ≤ 0   | 2,517  |
| Invalid Revenue | 11,805 |

---

## Duplicate Data

| Validation     | Total |
| -------------- | ----- |
| Duplicate Rows | 5,268 |

---

# 🧹 Data Cleaning Result

Several cleaning processes were performed:

* Removing missing values
* Removing invalid transactions
* Removing duplicate data
* Creating revenue column
* Converting datetime format

---

## Dataset After Cleaning

| Information           | Value   |
| --------------------- | ------- |
| Rows Before Cleaning  | 541,909 |
| Rows After Cleaning   | 392,692 |
| Clean Dataset Columns | 10      |

---

# 📊 Exploratory Data Analysis (EDA)

---

# 🛒 Top Product Analysis

## Best-Selling Products

Products with the highest quantity sold:

* PAPER CRAFT , LITTLE BIRDIE
* MEDIUM CERAMIC TOP STORAGE JAR
* JUMBO BAG RED RETROSPOT

---

## Highest Revenue Products

Products generating the highest revenue:

* PAPER CRAFT , LITTLE BIRDIE
* REGENCY CAKESTAND 3 TIER
* WHITE HANGING HEART T-LIGHT HOLDER

---

# 💰 Revenue Analysis

## Total Revenue

| Metric        | Value         |
| ------------- | ------------- |
| Total Revenue | 8,887,208.894 |

---

## Top Revenue Countries

Countries contributing the highest revenue:

1. United Kingdom
2. Netherlands
3. EIRE
4. Germany
5. France

---

## Revenue Trend Insights

* Highest revenue occurred during October and November 2011.
* Revenue fluctuates significantly across months.
* Strong seasonal purchasing patterns were identified.

---

# 🌍 Country Analysis

## Key Findings

* United Kingdom dominates both transactions and customer count.
* Germany and France are important international markets.
* International customers contribute significantly to company revenue.

---

# 📈 Sales Trend Analysis

## Key Findings

* Significant sales increase occurred between September and November 2011.
* November 2011 recorded the highest sales performance.
* Seasonal trends strongly affect company revenue.

---

# 👥 RFM Customer Segmentation

## 📌 RFM Analysis

RFM Analysis was used to segment customers based on:

* **Recency**
* **Frequency**
* **Monetary**

---

## Customer Segments

Customers were grouped into:

* Champions
* Loyal Customers
* Potential Customers
* At Risk Customers

---

## Segmentation Insights

* Champions represent the highest-value customers.
* Loyal customers contribute consistently to revenue.
* At Risk customers require retention strategies.
* Potential Customers can be targeted through promotions.

---

# 🌍 Customer Distribution Analysis

## Key Findings

* Most customers come from the United Kingdom.
* European countries contribute significantly to customer growth.
* Customer distribution analysis supports market expansion strategies.

---

# ☁️ Database Integration

The cleaned dataset and RFM dataset were uploaded to PostgreSQL Supabase for business intelligence integration.

Uploaded tables:

* `online_retail`
* `rfm_customer`

---

# 📊 Business Intelligence Dashboard

Dashboard developed using:

* [Metabase Official Website](https://www.metabase.com)
* PostgreSQL Supabase Integration

---

## Dashboard Components

* KPI Revenue
* Revenue by Country
* Top Products Analysis
* Monthly Sales Trend
* Customer Distribution
* RFM Customer Segmentation
* Revenue Trend Dashboard

---

# 📌 Business Insights

## Main Insights

* United Kingdom is the primary market contributor.
* Several products dominate both sales quantity and revenue.
* Strong seasonal sales patterns significantly impact revenue.
* RFM segmentation successfully identifies high-value customers.
* Customer distribution analysis helps optimize business strategies.

---

# 🚀 Business Recommendations

* Focus retention programs on loyal customers.
* Increase promotions during seasonal peak periods.
* Optimize inventory for best-selling products.
* Expand marketing to international markets.
* Use RFM segmentation for personalized marketing campaigns.

---

# 📁 Project Structure

```bash
├── data/
│   ├── Online Retail.xlsx
│   ├── clean_online_retail.csv
│   └── rfm_customer.csv
│
├── notebooks/
│   └── retail_analysis.ipynb
│
├── dashboard/
│   └── metabase_dashboard.png
│
├── README.md
└── requirements.txt
```




This project is intended for educational, research, and portfolio purposes.
