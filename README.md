# 📊 Online Retail Insights Dashboard

![Dashboard Preview](https://github.com/bhaskarpal1707/Online-Retail-Insights-Dashboard/blob/main/Dashboard%20Preview.png)

---

## 🎯 Purpose of the Project

The goal of this project is to build a comprehensive Power BI dashboard that delivers deep insights into the performance of an online retail platform. The dashboard enables business users to monitor sales, understand customer behavior, track product performance, and make data-driven decisions with confidence.

It combines sales, customer, product, and location data to provide a 360° view of the online retail operation.

---

## ✅ Outcome

- A fully interactive Power BI dashboard with dynamic slicers and visual filters.
- Key performance indicators (KPIs) for real-time business monitoring.
- Visualizations that spotlight trends, sales hotspots, and high-performing products.
- A clean, professional layout suitable for presentations, executive reviews, and strategic planning.

---
![Image1](https://github.com/bhaskarpal1707/Online-Retail-Insights-Dashboard/blob/main/Image1.jpg)

## 🚀 Project Overview

This dashboard integrates key datasets including orders, customers, products, payments, and geolocation to provide actionable insights for decision-makers in online retail.

It is designed to answer the following business questions:

- What are the total sales and average order values?
- How many unique customers and orders do we have?
- Which payment methods are most used?
- What product categories sell the most?
- Where are sales concentrated geographically?
- What are the top-performing products?
- How do sales trend over time?

---

## 📦 Data Model

The model integrates the following tables:

- `customers`
- `orders`
- `order_items`
- `products`
- `payments`
- `sellers`
- `geolocation`

![Image2](https://github.com/bhaskarpal1707/Online-Retail-Insights-Dashboard/blob/main/Image2.jpg)
---

## 📈 KPIs

### 1. 🛒 Total Sales
**DAX**: `Total Sales = SUM(order_items[price])`

**Insight**: Captures total revenue generated. It is the primary financial indicator of business performance.

---

### 2. 👥 Total Customers
**DAX**: `Total Customers = DISTINCTCOUNT(customers[customer_id])`

**Insight**: Measures the reach and scale of the customer base. Helps identify customer acquisition trends.

---

### 3. 📦 Total Orders
**DAX**: `Total Orders = DISTINCTCOUNT(orders[order_id])`

**Insight**: Represents total demand. Useful for assessing sales velocity and platform engagement.

---

### 4. 💳 Average Order Value (AOV)
**DAX**: `AOV = [Total Sales] / [Total Orders]`

**Insight**: Indicates the average revenue per transaction. A critical metric for pricing, promotions, and upselling strategies.

---
![Image3](https://github.com/bhaskarpal1707/Online-Retail-Insights-Dashboard/blob/main/Image3.jpg)
## 📊 Visualizations

### 1. 🧾 Payment Type Distribution
**Type**: Donut / Pie Chart  
**Fields**: `payments[payment_type]`, `SUM(payments[payment_value])`

**Insight**: Helps understand customer payment preferences (e.g., credit card, debit, vouchers). Aids in payment method optimization.

---

### 2. 🛍️ Product Category vs Quantity Sold
**Type**: Bar Chart  
**Fields**: `products[product_category]`, `COUNT(order_items[order_item_id])`

**Insight**: Highlights high-demand categories. Useful for inventory planning, marketing focus, and category expansion.

---

### 3. 🌍 Total Sales by Geolocation City
**Type**: Map or Tree Map  
**Fields**: `geolocation[geolocation_city]`, `SUM(order_items[price])`

**Insight**: Shows which cities generate the most revenue. Helps in targeting campaigns and logistics planning.

---

### 4. ⭐ Top 5 Selling Products
**Type**: Column Chart / Table  
**Fields**: `products[product_id]`, `SUM(order_items[price])`

**Insight**: Identifies best-sellers. Supports decisions on promotions, restocking, and product recommendations.

---

### 5. 📆 Sales Trends Over Time
**Type**: Line Chart  
**Fields**: `orders[order_purchase_timestamp]`, `SUM(order_items[price])`

**Insight**: Tracks revenue over time to detect seasonality, marketing impact, and growth trends.

---

## 🎛️ Slicers (Filters)

### 🔍 Customer City
**Field**: `customers[customer_city]`  
**Purpose**: Enables city-level analysis of customer behavior.

---

### 📂 Product Category
**Field**: `products[product_category]`  
**Purpose**: Allows focused analysis on specific product lines or verticals.

---

![Image4](https://github.com/bhaskarpal1707/Online-Retail-Insights-Dashboard/blob/main/Image4.jpg)
---

## 📌 Business Value

This dashboard enables stakeholders to:

- Understand where revenue comes from and what drives it.
- Make informed inventory, pricing, and marketing decisions.
- Spot growth opportunities across cities or product lines.
- Track financial and customer metrics over time.

---

## 🛠️ Tools Used

- Power BI Desktop
- DAX for KPI calculations
- Relational data modeling

---

## 📬 Contact

For questions or feedback, feel free to reach out via GitHub Issues or bhaskarpal.official@gmail.com.

---
