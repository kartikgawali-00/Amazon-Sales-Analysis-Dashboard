# 🛒 Amazon Sales Analysis Dashboard

<p align="center">

<img src="https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black">

<img src="https://img.shields.io/badge/Excel-Data%20Preparation-green">

<img src="https://img.shields.io/badge/Data%20Analytics-Business%20Insights-blue">

<img src="https://img.shields.io/badge/Project-Interactive%20Dashboard-orange">

</p>

---

# 📌 Project Overview

The **Amazon Sales Analysis Dashboard** is an interactive Business Intelligence project developed using **Power BI** to analyze Amazon sales performance, delivery operations, fulfillment efficiency, product demand, and regional sales distribution.

This dashboard converts raw sales data into meaningful business insights that help monitor order status, identify top-performing products, evaluate logistics performance, and understand customer purchasing patterns.

---
# 📂 Dataset Used

📊 **Dataset Link**

<a href="https://github.com/kartikgawali-00/Amazon-Sales-Analysis-Dashboard/blob/main/Amazon-Sales-Report-80K-Rows.xlsx">Dataset.csv</a>

---
# 🎯 Project Objective

The objective of this project is to analyze Amazon sales data and provide actionable insights into:

✅ Sales Performance

✅ Order Status Tracking

✅ Product Category Analysis

✅ Size-wise Demand Analysis

✅ Fulfillment Performance

✅ Delivery Partner Analysis

✅ Regional Sales Distribution

✅ Operational Efficiency

The dashboard enables stakeholders to make data-driven decisions for improving sales and logistics performance.

---

# 🛠️ Tools & Technologies Used

| Technology | Purpose |
|------------|----------|
| 📊 Power BI | Dashboard Development |
| 📑 Excel | Data Cleaning & Preparation |
| ⚡ DAX | KPI & Measure Creation |
| 🔄 Power Query | Data Transformation |
| 📈 Data Visualization | Business Insights |

---

# 📂 Dataset Information

The dataset contains Amazon sales and order-related information including:

* Order ID
* Order Date
* Product Category
* Product Size
* Sales Amount
* Courier Status
* Fulfillment Type
* Delivery Partner
* Ship State
* Quantity
* Order Status

---

# 📊 Dashboard Overview

## 📈 Key KPIs

| KPI | Value |
|------|--------|
| 💰 Total Sales Amount | 29.01M |
| 📅 Analysis Period | Apr 2022 - May 2022 |
| 📦 Shipped Orders | 40.35K |
| 🚚 Orders On The Way | 2.86K |
| ❌ Cancelled Orders | 1.95K |
| ⏳ Unshipped Orders | 593 |

---

# 📊 Dashboard Components

## 1️⃣ Sales Overview

### Business Questions

* What is the total sales revenue generated?
* How many orders were successfully shipped?
* What is the overall order fulfillment performance?
* How effective is the delivery process?

### Key Insights

✅ Total sales reached **29.01 Million**.

✅ Most orders were successfully shipped.

✅ Cancellation and unshipped rates remain relatively low.

✅ The sales trend indicates strong customer demand.

---

## 2️⃣ Courier Status Analysis

### Visualizations Used

* Courier Status Pie Chart
* Order Distribution by Status

### Courier Status Breakdown

| Status | Orders |
|----------|---------|
| Shipped | 40.35K |
| On The Way | 2.86K |
| Cancelled | 1.95K |
| Unshipped | 593 |

### Key Insights

✅ Approximately 86% of orders were successfully shipped.

✅ A small percentage of orders were cancelled.

✅ Unshipped orders require operational monitoring.

---

## 3️⃣ Product Category Analysis

### Top Categories

| Category | Performance |
|------------|------------|
| 👕 T-Shirt | Highest Demand |
| 👖 Trousers | High Demand |
| 👛 Wallet | Moderate Demand |
| 🧦 Socks | Low Demand |
| 👟 Shoes | Low Demand |

### Key Insights

✅ T-Shirts contribute the highest sales volume.

✅ Apparel products dominate overall demand.

✅ Accessories contribute a smaller share of total sales.

---

## 4️⃣ Fulfillment Analysis

### Fulfillment Types

* Amazon Fulfilled
* Merchant Fulfilled

### Key Insights

✅ Amazon Fulfillment handles the majority of orders.

✅ Merchant Fulfillment contributes a smaller share.

✅ Centralized fulfillment improves delivery efficiency.

---

## 5️⃣ Delivery Partner Analysis

### Delivery Partners

* Ekart
* Easy Ship

### Key Insights

✅ Ekart processes the highest number of deliveries.

✅ Easy Ship serves as an important secondary logistics partner.

✅ Delivery performance directly impacts customer satisfaction.

---

## 6️⃣ Product Size Analysis

### Size-wise Demand

| Size | Demand |
|--------|---------|
| M | Highest |
| XL | High |
| XXL | Moderate |
| L | Moderate |
| S | Lower |
| XS | Lowest |

### Key Insights

✅ Medium-sized products are the most preferred.

✅ XL and XXL sizes show strong customer demand.

✅ XS products have the lowest sales volume.

---

## 7️⃣ State-wise Sales Analysis

### Top Performing States

1. Maharashtra
2. Karnataka
3. Tamil Nadu
4. Telangana
5. Uttar Pradesh

### Business Questions

* Which states generate the highest order volume?
* How is demand distributed geographically?
* Which regions contribute most to overall sales?

### Key Insights

✅ Maharashtra records the highest number of orders.

✅ Southern states contribute significantly to total sales.

✅ Urban and densely populated regions drive the majority of demand.

---
### Dashboard Preview

# 📂 Dataset Used

📊 **Dataset Link:**  
<img src="https://github.com/kartikgawali-00/Amazon-Sales-Analysis-Dashboard/blob/main/Dashboard%20Image/Screenshot%202026-06-01%20182442.png?raw=true">

---

# 📈 DAX Measures


### Total Sales

```DAX
Total Sales =
SUM(Amazon[Amount])
```

### Total Orders

```DAX
Total Orders =
COUNT(Amazon[Order ID])
```

### Shipped Orders

```DAX
Shipped Orders =
CALCULATE(
    COUNT(Amazon[Order ID]),
    Amazon[Courier Status] = "Shipped"
)
```

### Cancelled Orders

```DAX
Cancelled Orders =
CALCULATE(
    COUNT(Amazon[Order ID]),
    Amazon[Courier Status] = "Cancelled"
)
```

### Cancellation Rate

```DAX
Cancellation Rate =
DIVIDE(
    [Cancelled Orders],
    [Total Orders]
)
```

---

# 💡 Project Insights

## 🛒 Sales Insights

* Total sales exceeded **29 Million**.
* Apparel products drive the majority of revenue.
* T-Shirts are the highest-selling category.

## 📦 Operations Insights

* Most orders are successfully shipped.
* Amazon Fulfillment handles the majority of deliveries.
* Operational efficiency remains strong.

## 🚚 Logistics Insights

* Ekart is the primary delivery partner.
* Cancellation and unshipped rates are low.
* Delivery performance can be further optimized through proactive monitoring.

## 🌍 Regional Insights

* Maharashtra leads in order volume.
* Karnataka and Tamil Nadu are major contributors.
* Demand is concentrated in metropolitan regions.

---

# 🚀 Business Recommendations

### 📈 Inventory Optimization

Maintain higher stock levels for:

* T-Shirts
* Medium (M) Size
* XL Size Products

### 🚚 Improve Logistics Monitoring

Reduce delivery delays by tracking orders that remain unshipped for extended periods.

### 🎯 Regional Marketing

Focus promotional campaigns in high-performing states:

* Maharashtra
* Karnataka
* Tamil Nadu

### 📦 Strengthen Fulfillment Operations

Increase utilization of Amazon Fulfillment to improve delivery performance.

### 🛍️ Category Expansion

Expand inventory for top-performing apparel categories to maximize sales opportunities.

---

# 📷 Dashboard Preview

![Amazon Sales Dashboard](images/Amazon_Sales_Dashboard.png)

---

# 🏆 Skills Demonstrated

### 📊 Power BI

* Interactive Dashboard Design
* KPI Development
* DAX Measures
* Data Modeling
* Data Visualization
* Business Intelligence Reporting

### 📑 Excel

* Data Cleaning
* Data Validation
* Data Preparation

### 📈 Analytics

* Sales Analysis
* Customer Demand Analysis
* Logistics Analysis
* Geographic Analysis
* Performance Reporting

---

# 📌 Final Conclusion

The Amazon Sales Analysis Dashboard provides a comprehensive overview of sales performance, order fulfillment, logistics operations, product demand, and regional sales distribution.

The analysis highlights strong demand for apparel products, high sales concentration in key Indian states, efficient fulfillment processes, and opportunities to further optimize inventory and logistics operations. These insights support better business decisions and improved operational efficiency.

---

# 👨‍💻 Author

## Kartik Gawali

📊 Data Analyst | Power BI | Excel | Data Visualization

⭐ If you found this project useful, don't forget to star the repository.
