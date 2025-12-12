# 🚲 Jenson USA Sales Analysis: SQL Case Study

![SQL](https://img.shields.io/badge/Language-MySQL-blue?style=for-the-badge&logo=mysql)
![Data Analysis](https://img.shields.io/badge/Focus-Window_Functions-orange?style=for-the-badge)
![E-Commerce](https://img.shields.io/badge/Domain-Retail_Sales-green?style=for-the-badge)

## 🎯 Project Overview
Jenson USA is a leading retailer of bicycles, parts, and accessories. This project involves a deep-dive analysis of their sales database using **Advanced SQL**. The goal was to optimize inventory, evaluate staff performance, and identify high-value customer segments.

## 🗂️ Dataset & Schema
The analysis involved complex relationships between multiple tables:
* **Sales Data:** `orders`, `order_items`
* **Inventory:** `products`, `categories`, `brands`, `stocks`
* **Operations:** `stores`, `staffs`
* **Customers:** `customers`

---

## 💻 Advanced SQL Solutions
I solved 12 complex business problems using advanced techniques:

### 1. 📈 Advanced Sales Analysis (Window Functions)
* **Cumulative Trends:** Calculated the running total of quantities sold for products over time using `SUM() OVER(PARTITION BY... ORDER BY...)`.
* **Category Leaders:** Identified the highest-grossing product in *each* category using `ROW_NUMBER()`.
* **Median Pricing:** Implemented a statistical logic to find the **Median Price** of the product list (a calculation not natively available in basic SQL).

### 2. 👥 Staff & Store Performance
* **Underperforming Staff:** Used `NOT EXISTS` to find staff members who have never made a sale.
* **Top Performers (CTE):** Used a Common Table Expression (CTE) to identify staff members whose sales exceeded the **average sales** of all staff.
* **Store Metrics:** Calculated total product volume sold by each store location.

### 3. 🛍️ Customer & Product Insights
* **High-Value Customers:** Ranked customers by total spend using `RANK()`.
* **Inventory Gaps:** Identified products that have **never been ordered** using `NOT EXISTS` to assist with inventory clearing decisions.
* **Super Users:** Identified unique customers who have ordered products from **every single category** available (Complex Join + Aggregation).

---

## 🛠️ Technical Skills Demonstrated
* **Window Functions:** `RANK()`, `DENSE_RANK()`, `ROW_NUMBER()`, `SUM() OVER()`.
* **CTEs (Common Table Expressions):** Used `WITH` clauses for cleaner, more readable complex queries.
* **Statistical Analysis:** Calculating Median and Cumulative sums.
* **Subqueries:** Used `NOT EXISTS` and nested subqueries for filtering.

---

## ✅ Business Impact
* **Inventory Optimization:** Identified unsold inventory and fast-moving categories.
* **Staff Training:** Highlighted underperforming staff for potential training programs.
* **Pricing Strategy:** Analyzed price distributions (Median vs Average) to understand product positioning.

---
