# Retail Inventory & Supply Chain Analytics

## 📊 Project Overview

Retail Inventory & Supply Chain Analytics is a Power BI project developed for **MegaMart Retail Pvt. Ltd.** to analyze inventory levels, product replenishment, warehouse performance, supplier performance, and inventory movement.

The project transforms raw Excel inventory data into an interactive business intelligence dashboard using **Power Query, Star Schema, DAX, and Power BI visualizations**.

---

## 🎯 Project Objectives

- Analyze overall inventory value and stock quantity.
- Identify products requiring replenishment.
- Monitor warehouse stock levels and capacity utilization.
- Analyze supplier lead times and purchase performance.
- Identify categories with higher inventory turnover.
- Analyze monthly inventory and purchase movement.
- Identify dead-stock products.
- Provide business recommendations for improving inventory efficiency and reducing costs.

---

## 🗂️ Dataset

The project uses Excel-based inventory and master data.

### Fact Table

- **Fact_Inventory** – 5,010 records

### Dimension Tables

- **Dim_Product** – 300 products
- **Dim_Category** – 12 categories
- **Dim_Supplier** – 60 suppliers
- **Dim_Warehouse** – 15 warehouses
- **Dim_Location** – 12 locations
- **Dim_Date** – Date dimension

---

## 🔄 Data Cleaning & Transformation

Data preparation was performed using **Power Query**.

### Key Activities

- Removed duplicate records.
- Corrected data types.
- Cleaned transaction dates.
- Handled invalid expiry-date values.
- Standardized Payment Mode values.
- Checked missing values and errors.
- Prepared fact and dimension tables for data modeling.

---

## 🏗️ Data Model

A **Star Schema** was implemented in Power BI.

### Fact Table

`Fact_Inventory`

### Dimension Tables

text
                 Dim_Product
                      |
                 Dim_Category
                      |
Dim_Supplier — Fact_Inventory — Dim_Warehouse
                      |
                 Dim_Location
                      |
                   Dim_Date


🧮 DAX Measures

The following DAX measures were created:

Total Stock Quantity
Inventory Value
Total Purchase Quantity
Total Purchase Value
Total Reorder Quantity
Stock-out Rate
Dead Stock %
Average Lead Time
Average Inventory Value
Inventory Turnover
YTD Purchase Value
Low Stock Count
Out of Stock Count

🔍 Business Questions & Answers
1. Which products have the highest inventory value?

The products with the highest inventory value include:

Bakery Product 26
Home Care Product 151
Health Product 264
Home Care Product 283
Beverages Product 15

2. Which products require immediate replenishment?

The products with the highest reorder quantities include:

Groceries Product 293
Dairy Product 25
Frozen Foods Product 250
Frozen Foods Product 118
Dairy Product 1

3. Which warehouses have excess or insufficient stock?

Warehouse stock pressure was analyzed using stock quantity, reorder requirements, stock status, and capacity utilization.

Coimbatore Overflow DC shows high stock pressure with 95% utilization and the highest reorder requirement.
Chennai Regional DC operates at 97% utilization.
Madurai Warehouse has a relatively high number of low-stock records.
Hosur Logistics Hub has high stock levels and 90% utilization.

Note: The project data does not define a separate formal threshold for "excess stock" or "insufficient stock", so these observations are based on available stock, reorder, and utilization indicators.

4. Which suppliers have the longest lead time?

Suppliers with the longest lead times include:

Supplier	Lead Time
Supplier 18	28 days
Supplier 58	20 days
Supplier 55	20 days
Supplier 29	20 days
Supplier 57	20 days

Supplier 18 has the longest recorded lead time at 28 days.

5. Which categories have the fastest inventory turnover?

The categories with the highest inventory turnover include:

Bakery
Snacks
Groceries
Stationery
Fruits & Vegetables

Bakery has the highest calculated inventory turnover.

6. What is the monthly inventory movement trend?

Monthly purchase activity fluctuates throughout the year.

March recorded the highest purchase value at approximately ₹63.18 million.
September recorded approximately ₹62.43 million.
April recorded the lowest purchase value at approximately ₹50.21 million.

Overall, the data shows monthly fluctuations rather than a sustained upward or downward trend.

7. Which products are slow-moving or dead stock?

Using Current Stock = 0 as the project's dead-stock definition, the identified dead-stock products are:

Personal Care Product 6
Bakery Product 26
Fruits & Vegetables Product 95
Frozen Foods Product 106
Beverages Product 135
Snacks Product 232
Groceries Product 293

The dataset does not define a separate quantitative threshold for slow-moving stock.

💡 Business Recommendations
Prioritize replenishment for products with high reorder quantities.
Monitor warehouses operating at high capacity utilization.
Review suppliers with longer lead times.
Monitor high-value inventory to control carrying costs.
Improve demand forecasting for frequently purchased categories.
Investigate products with zero current stock.
Consider inventory redistribution between warehouses where appropriate.
Monitor monthly purchase patterns for better procurement planning.

🛠️ Tools & Technologies
Microsoft Power BI
Power Query
DAX
Microsoft Excel
Data Modeling
Star Schema
Data Analysis
Business Intelligence
Data Visualization

📌 Power BI Features Used
KPI Cards
Slicers
Matrix
Bar Charts
Column Charts
Line Charts
Donut Charts
Conditional Formatting
Drill-through
Report Page Tooltips
Bookmarks
Page Navigation
Interactive Filtering

👨‍💻 My Role

Role: BI Analyst

Responsibilities
Data cleaning and transformation
Power Query ETL
Data modeling
Star Schema implementation
DAX measure development
Power BI dashboard development
Business analysis
Insight generation
Business recommendations


