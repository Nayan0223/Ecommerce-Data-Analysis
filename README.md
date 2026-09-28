# 🛒 E-Commerce Data Analysis

```{=html}
<p align="center">
```
`<b>`{=html}End-to-End Data Analytics Project using Python, Pandas,
Seaborn, Matplotlib & Power BI`</b>`{=html}
```{=html}
</p>
```
```{=html}
<p align="center">
```
`<img src="https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white">`{=html}
`<img src="https://img.shields.io/badge/Pandas-Data%20Cleaning-150458?style=for-the-badge&logo=pandas&logoColor=white">`{=html}
`<img src="https://img.shields.io/badge/Seaborn-EDA-4C72B0?style=for-the-badge">`{=html}
`<img src="https://img.shields.io/badge/Matplotlib-Visualization-11557C?style=for-the-badge">`{=html}
`<img src="https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black">`{=html}
```{=html}
</p>
```

------------------------------------------------------------------------

## 📌 Overview

An end-to-end **E-Commerce Data Analysis** project covering:

**Data Understanding → Data Cleaning → Validation → EDA → Visualization
→ Business Insights → Dashboard Preparation**

The project transforms transactional data into an analysis-ready dataset
and explores sales, products, channels, geography, pricing, and order
status.

## 🎯 Objectives

-   Clean and validate e-commerce transaction data
-   Analyze revenue trends
-   Identify high-performing products
-   Compare sales channels
-   Analyze country-level performance
-   Understand completed vs refunded orders
-   Explore quantity vs unit price
-   Prepare data for Power BI

## 📊 Dataset

The original dataset contains **3,047 records and 13 columns**.

  Column             Description
  ------------------ ---------------------------
  `order_id`         Order identifier
  `order_date`       Order date
  `customer_email`   Customer email identifier
  `country`          Country
  `channel`          Sales channel
  `product_sku`      Product SKU
  `product_name`     Product
  `quantity`         Quantity ordered
  `unit_price`       Unit price
  `order_total`      Recorded order total
  `weight`           Weight
  `currency`         Transaction currency
  `status`           Order status

> ⚠️ The source contains EUR and GBP. Revenue should not be directly
> compared across currencies without a documented currency-conversion
> step.

## 🧹 Data Cleaning

The project includes:

-   Missing-value analysis
-   Duplicate detection
-   Duplicate order-ID checks
-   Data-type conversion
-   Text standardization
-   Mixed date-format conversion
-   Numeric conversion
-   Invalid quantity detection
-   Invalid price detection
-   Revenue calculation
-   Order-total validation

### Missing Price Treatment

Missing `unit_price` values were investigated instead of filling them
with zero.

Where possible:

``` text
Recovered Unit Price = Order Total / Quantity
```

Then:

``` text
Calculated Revenue = Quantity × Unit Price
```

## 🔎 Exploratory Data Analysis

### 📈 Monthly Revenue Trend

![Monthly Revenue Trend](01_monthly_revenue_trend.png)

### 🏆 Top 10 Products by Revenue

![Top Products](02_top_10_products_revenue.png)

### 📣 Revenue by Sales Channel

![Sales Channel](03_revenue_by_sales_channel.png)

### 🌍 Revenue by Country

![Country Revenue](04_revenue_by_country.png)

### 🔎 Quantity vs Unit Price

![Quantity vs Price](05_quantity_vs_unit_price.png)

### 📦 Order Status Distribution

![Order Status](06_order_status_distribution.png)

### 📊 Revenue Distribution

![Revenue Distribution](07_revenue_distribution.png)

### 🔗 Correlation Matrix

![Correlation Matrix](08_correlation_heatmap.png)

## 📌 Initial Data-Quality Findings

  Check                                    Finding
  -------------------------------------- ---------
  Original records                           3,047
  Duplicate rows                                47
  Duplicate order IDs                           47
  Missing unit prices before treatment         228
  Non-positive quantities                      102
  Initial order-total mismatches               208

## 🛠️ Tech Stack

**Python:** Pandas, NumPy

**Visualization:** Matplotlib, Seaborn

**BI:** Power BI

**Environment:** Jupyter Notebook

**Version Control:** Git & GitHub

## 📁 Project Structure

``` text
Ecommerce-Data-Analysis/
│
├── ecommerce_analysis.ipynb
├── ecommerce_cleaned.csv
├── README.md
├── LICENSE
│
├── 01_monthly_revenue_trend.png
├── 02_top_10_products_revenue.png
├── 03_revenue_by_sales_channel.png
├── 04_revenue_by_country.png
├── 05_quantity_vs_unit_price.png
├── 06_order_status_distribution.png
├── 07_revenue_distribution.png
└── 08_correlation_heatmap.png
```

## 🚀 Run Locally

``` bash
git clone https://github.com/Nayan0223/Ecommerce-Data-Analysis.git
cd Ecommerce-Data-Analysis
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook
```

Open:

``` text
ecommerce_analysis.ipynb
```

Run the notebook from top to bottom.

## 📈 Power BI Dashboard Plan

### KPI Cards

-   Total Orders
-   Total Revenue
-   Total Customers
-   Average Order Value
-   Refund Rate
-   Total Quantity

### Visuals

-   Monthly Revenue Trend
-   Revenue by Country
-   Revenue by Channel
-   Top Products
-   Order Status
-   Quantity vs Unit Price
-   Currency-aware revenue analysis

### Filters

-   Date
-   Country
-   Channel
-   Product
-   Status
-   Currency

## 🧠 Skills Demonstrated

`Python` · `Pandas` · `NumPy` · `SQL` · `Excel` · `Power BI` · `Seaborn`
· `Matplotlib` · `EDA` · `Data Cleaning` · `Data Validation`

## 👨‍💻 Author

**Nayan Bharodiya**

BCA Graduate \| Aspiring Data Analyst

## ⭐ Project Goal

> **Turn messy transactional data into reliable, understandable, and
> business-ready insights.**

If you find this project useful, consider giving the repository a ⭐.

## 📜 License

MIT License
