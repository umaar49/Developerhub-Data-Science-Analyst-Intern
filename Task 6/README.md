# 📌 Online Retail Store Analysis & Dashboard

## 📖 Introduction

This project analyzes an **Online Retail dataset** to extract business insights through exploratory data analysis (EDA) and interactive visualizations. The focus is on understanding customer behavior, product performance, and sales patterns across different time periods. Additionally, a dashboard is built using **Streamlit** and **Plotly** to make the analysis interactive and user-friendly.

---

## 📂 Dataset

* **Dataset Used:** Online Retail dataset (filtered version from **Task 1**)
* **Description:** Contains transactions from an online retail store, including customer IDs, product descriptions, quantities, prices, dates, and countries.
* **Target Use:** To understand sales trends, customer segmentation, and product performance for business decision-making.

---

## ⚙️ Data Preprocessing & Handling

1. **Missing and Null Values:** Identified and handled missing records.
2. **Duplicate Records:** Removed duplicates to ensure data consistency.
3. **Invalid Values:** Dropped rows with `UnitPrice <= 0` or negative values.
4. **Data Type Conversion:** Converted `InvoiceDate` from object type to **datetime** for time-based analysis.
5. **Filtered Dataset:** Used the already preprocessed dataset from Task 1 for consistency.

---

## 🔎 Exploratory Data Analysis (EDA)

Key analysis steps performed:

* **Monthly Sales Trends** – Tracked sales growth and seasonality over time.
* **Hourly Sales Distribution** – Analyzed peak sales hours in a day.
* **Top 10 Products by Sales** – Found the highest revenue-generating products.
* **Trending Products by Month** – Observed product popularity changes across months.
* **Top 10 Countries by Sales** – Discovered leading international markets outside the UK.

---

## 📊 Dashboard Creation

An **interactive dashboard** was developed using:

* **Streamlit** – To create a web-based interactive user interface.
* **Plotly** – For dynamic and interactive data visualizations.

The dashboard includes visual insights for:

* Monthly Sales
* Hourly Sales
* Top Customers
* Top Products
* Country-wise Sales

---

## 🧠 Technologies & Libraries Used

* **Python**
* **Pandas** – Data manipulation & preprocessing
* **NumPy** – Numerical computations
* **Matplotlib & Seaborn** – Exploratory visualizations
* **Plotly** – Interactive plots for dashboard
* **Streamlit** – Dashboard and web application

---
* Dashboard Link(https://retailstoredashboard.streamlit.app/)

