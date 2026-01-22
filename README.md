📦 Supply Chain & Inventory Analysis Project
📌 Project Overview

This project analyzes supply chain and inventory data to identify inefficiencies in stock management, supplier performance, warehouse operations, and order fulfillment.
Using SQL, Python, and Power BI, the project provides actionable insights to improve operational efficiency and reduce business risks such as stockouts and delivery delays.

🎯 Project Objectives

Analyze inventory levels across warehouses

Identify understock and overstock products

Evaluate supplier performance and lead times

Measure warehouse efficiency and delivery delays

Build interactive dashboards for business decision-making

Generate data-driven insights using SQL and Power BI

🗂️ Dataset Description

The project uses four datasets in CSV format.

1️⃣ Orders (orders.csv)

Contains information about customer orders and delivery timelines.

Column Name	Description
order_id	Unique order identifier
order_date	Date when the order was placed
product_id	Product identifier
warehouse_id	Warehouse identifier
quantity_ordered	Quantity ordered
customer_region	Customer region
expected_delivery_date	Expected delivery date
delivery_date	Actual delivery date

2️⃣ Products (products.csv)

Contains product-related details.

Column Name	Description
product_id	Product identifier
product_name	Product name
category	Product category
unit_cost	Cost per unit
unit_price	Selling price per unit

3️⃣ Inventory (inventory.csv)

Contains stock information across warehouses.

Column Name	Description
product_id	Product identifier
warehouse_id	Warehouse identifier
stock_on_hand	Current stock quantity
reorder_level	Minimum stock threshold
reorder_quantity	Quantity to reorder
last_updated	Last updated date

4️⃣ Suppliers (suppliers.csv)

Contains supplier performance data.

Column Name	Description
supplier_id	Supplier identifier
product_id	Product supplied
lead_time_days	Delivery lead time (days)
supplier_rating	Supplier rating

🛠️ Tools & Technologies

SQL – Data analysis and KPI calculation

Python (Pandas) – Data cleaning and exploratory analysis

Power BI – Data visualization and dashboards

Excel – Data inspection and preprocessing

📊 Key KPIs & Metrics
📦 Inventory Metrics

Inventory Turnover Ratio

Understock & Overstock Products

Stock Status (Understock / Optimal / Overstock)

Lost Sales due to Stockouts

🚚 Supply Chain Metrics

On-Time Delivery Percentage

Average Delivery Delay

Warehouse-wise Performance

Region-wise Order Distribution

🏭 Supplier Metrics

Average Lead Time

Supplier Rating

Supplier Performance Score

Delay Impact by Supplier

🧮 SQL Analysis

SQL was used to perform:

Data joins across multiple tables

Aggregations using GROUP BY

Conditional logic using CASE

KPI calculations for supply chain performance

Example SQL query:

SELECT 
    ROUND(100.0 * SUM(CASE WHEN delivery_date <= expected_delivery_date THEN 1 ELSE 0 END) / COUNT(*), 2) 
    AS on_time_delivery_percentage
FROM orders;

📈 Power BI Dashboard

The Power BI report consists of four main pages:

1️⃣ Executive Overview

Total Orders

Total Revenue

On-Time Delivery %

Inventory Turnover

Sales and order trends

2️⃣ Inventory Analysis

Stock levels by product and warehouse

Understock and overstock analysis

Category-wise inventory distribution

3️⃣ Warehouse Performance

Average delivery delay by warehouse

Orders by warehouse

Delay trends over time

4️⃣ Supplier Performance

Lead time by supplier

Supplier rating vs lead time (scatter plot)

Supplier performance table

Best and worst suppliers identification

💡 Key Insights

Certain products frequently fall below reorder levels, increasing stockout risk.

Some warehouses consistently show higher delivery delays.

Suppliers with longer lead times negatively impact order fulfillment.

Overstocked products contribute to higher inventory holding costs.

Supplier ratings do not always align with actual delivery performance.

📌 Business Impact

This project demonstrates how data analytics can:

Optimize inventory management

Improve supplier selection and monitoring

Reduce delivery delays

Minimize lost sales

Support strategic supply chain decisions

🚀 Future Enhancements

Demand forecasting using machine learning

Real-time dashboard integration

Cost optimization analysis

Predictive supply chain modeling

👤 Author

Rishi Bhardwaj
Aspiring Data Analyst

Skills: SQL | Python | Power BI | Excel | Data Analysis
linkedin - www.linkedin.com/in/rishi-b-93b91b296
