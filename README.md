# 📊 Sales Dashboard – Power BI

## 📌 Project Overview

The **Sales Dashboard** is an interactive data visualization project developed using Microsoft Power BI. It helps analyze sales performance, profit, order volume, quantity sold, and sales distribution across different regions, customer segments, and product categories.

The dashboard provides a clear overview of business performance through KPI cards, charts, and interactive slicers.

## 🎯 Project Objectives

* Analyze overall sales and profit performance.
* Track the total number of orders and quantity sold.
* Compare sales across different regions.
* Understand sales distribution by customer segment.
* Analyze sales performance across product categories.
* Enable interactive filtering for better data exploration.

## 🛠️ Tools & Technologies

* **Microsoft Power BI** – Dashboard creation and visualization
* **Power Query** – Data cleaning and transformation
* **DAX (Data Analysis Expressions)** – Measures and calculations
* **Data Modeling** – Relationships between tables

## 📂 Dataset

The project uses a Superstore-style sales dataset containing information about orders, customers, products, sales, profits, discounts, and geographical regions.

Key fields include:

* Order ID and Order Date
* Customer ID and Customer Name
* Product ID and Product Name
* Sales, Profit, Quantity, and Discount
* Region, Category, and Sub-Category
* Segment, City, and Country

## 📈 Dashboard Features

### 1. Key Performance Indicators (KPIs)

* Total Sales
* Total Profit
* Total Orders
* Total Quantity

### 2. Sales Analysis Visualizations

* **Sales by Region:** Compares sales performance across geographical regions.
* **Sales by Segment:** Displays the contribution of different customer segments to total sales.
* **Sales by Category:** Compares sales across product categories.

### 3. Interactive Slicers

* Sub-Category
* Category
* Region

These slicers allow users to filter the dashboard and explore sales performance for specific groups.

## 🗂️ Data Model

The Power BI model contains the following tables:

* **Customer:** Customer details and customer IDs.
* **Product:** Product information, categories, and sub-categories.
* **Order:** Order details, sales, profit, quantity, and related transaction fields.
* **Date:** Date, year, month, and day-of-week information.
* **Measure:** A dedicated table for organizing DAX measures.
* **superstore_raw:** Original source dataset.

Relationships between the relevant tables help connect customer, product, and date information with order data.

## 🧮 DAX Measures

The following measures are used to calculate the dashboard KPIs:

```DAX
Total Sales =
SUM('Order'[Sales])
```

```DAX
Total Profit =
SUM('Order'[Profit])
```

```DAX
Total Orders =
DISTINCTCOUNT('Order'[Order ID])
```

```DAX
Total Quantity =
SUM('Order'[Quantity])
```

```DAX
Total Customers =
DISTINCTCOUNT('Customer'[Customer ID])
```

*Note: The table and column names in the DAX formulas should match the names in your Power BI model.*

## 🔍 Key Learnings

* Data cleaning and transformation using Power Query.
* Creating and managing relationships between tables.
* Writing DAX measures for business KPIs.
* Building interactive charts, cards, and slicers.
* Designing a structured and user-friendly dashboard.
* Understanding business performance through data visualization.

## 🚀 Conclusion

This project demonstrates how Power BI can transform raw sales data into an interactive dashboard that supports business performance analysis. It provides a consolidated view of key sales metrics and enables users to explore sales trends across regions, customer segments, and product categories.

## 👩‍💻 Author

**Akshaya A**

BCA Student | Aspiring Data Analyst | UI/UX Designer
