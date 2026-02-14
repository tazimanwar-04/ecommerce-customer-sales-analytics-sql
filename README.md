# 📊 E-Commerce Customer & Sales Analytics using SQL

## 📌 Project Overview

This project analyzes the Brazilian Olist E-Commerce dataset using MySQL to simulate real-world business analytics.

The objective was to design a relational database from raw CSV files, perform SQL-based business analysis, and generate actionable insights for decision-making.

---

## 🎯 Project Objectives

- Design a clean relational database schema
- Implement Primary & Foreign Key relationships
- Perform revenue and customer behavior analysis
- Identify geographic performance trends
- Measure customer retention and lifetime value
- Analyze delivery performance
- Generate business recommendations

---

## 🗂 Dataset Information

**Dataset Source:**  
Brazilian Olist E-Commerce Dataset (Kaggle)

**Core Tables Used:**
- `olist_orders`
- `olist_order_items`
- `olist_customer`
- `olist_products`

**Dataset Size:**
- 99,441 Orders
- 96,000+ Unique Customers
- 112,650 Order Items
- 32,949 Products

---

## 🧱 Database Design

- Designed relational schema using MySQL
- Implemented Primary Keys (PK)
- Implemented Foreign Keys (FK)
- Cleaned datetime fields using `STR_TO_DATE`
- Validated null values and data integrity
- Reverse engineered schema into ERD

📌 ERD diagram included in repository (`ERD.png`)

---

## 📈 Key Business Analysis Performed

### 1️⃣ Revenue Analysis
- Total Revenue Calculation
- Average Order Value (AOV)
- Monthly Revenue Trend

### 2️⃣ Product & Category Analysis
- Revenue by Product Category
- Top Products per Category (using Window Functions)
- Revenue Distribution Analysis

### 3️⃣ Customer Analytics
- Repeat vs New Customer Segmentation
- Customer Lifetime Value (CLV)
- Purchase Behavior Insights

### 4️⃣ Geographic Analysis
- Revenue by State
- Revenue Ranking using `RANK()`

### 5️⃣ Operational Analysis
- Delivery Delay Analysis
- Performance vs Estimated Delivery Dates

---

## 📊 Key Business Insights

### Revenue & Growth
- Total Revenue: 13.59M
- Strong growth during 2017
- Revenue peaked in November 2017 (~1M)
- Stabilized around 900K–1M monthly in 2018

### Customer Behavior
- Only ~3% customers are repeat buyers
- Business heavily dependent on new customer acquisition
- Significant opportunity for retention strategies

### Geographic Insights
- São Paulo contributes ~38% of total revenue
- Revenue concentrated in southeastern Brazil
- Expansion opportunity in underperforming regions

### Product Insights
- Top categories: Beauty & Health, Gifts, Home & Bedding
- Revenue well distributed across catalog
- No single product dependency risk

### Delivery Performance
- Orders delivered ~11 days earlier than estimated
- Strong logistics efficiency

---

## 🛠 SQL Techniques Used

- `JOIN`
- `GROUP BY`
- Aggregate Functions (`SUM`, `AVG`, `COUNT`)
- `CASE` Statements
- Common Table Expressions (CTE)
- Window Functions (`RANK()`)
- Date Formatting & Conversion
- `DATEDIFF` Analysis

---

## 📂 Repository Structure

