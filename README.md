📦 Supply Chain & Inventory Analysis Project

📌 Project Overview

This project analyzes supply chain and inventory data to identify inefficiencies in stock management, supplier performance, warehouse operations, and order fulfillment.
Using SQL, Python, and Power BI, the project provides actionable insights to improve operational efficiency and reduce business risks such as stockouts and delivery delays.

🎯 Project Objectives

   1) Analyze inventory levels across warehouses
   
   2) Identify understock and overstock products
   
   3) Evaluate supplier performance and lead times
   
   4) Measure warehouse efficiency and delivery delays
   
   5) Build interactive dashboards for business decision-making
   
   6) Generate data-driven insights using SQL and Power BI

🗂️ Dataset Description

The project uses four datasets in CSV format.

1️⃣ Orders (orders.csv)

Contains information about customer orders and delivery timelines.

Column Name	Description
   1) order_id	Unique order identifier
   2) order_date	Date when the order was placed
   3) product_id	Product identifier
   4) warehouse_id	Warehouse identifier
   5) quantity_ordered	Quantity ordered
   6) customer_region	Customer region
   7) expected_delivery_date	Expected delivery date
   8) delivery_date	Actual delivery date

2️⃣ Products (products.csv)

Contains product-related details.

Column Name	Description
   1) product_id	Product identifier
   2) product_name	Product name
   3) category	Product category
   4) unit_cost	Cost per unit
   5) unit_price	Selling price per unit

3️⃣ Inventory (inventory.csv)

Contains stock information across warehouses.

Column Name	Description
    1) product_id	Product identifier
    2) warehouse_id	Warehouse identifier
    3) stock_on_hand	Current stock quantity
    4) reorder_level	Minimum stock threshold
    5) reorder_quantity	Quantity to reorder
    6) last_updated	Last updated date

4️⃣ Suppliers (suppliers.csv)

Contains supplier performance data.

Column Name	Description
    1) supplier_id	Supplier identifier
    2) product_id	Product supplied
    3) lead_time_days	Delivery lead time (days)
    4) supplier_rating	Supplier rating

🛠️ Tools & Technologies

    SQL – Data analysis and KPI calculation
    
    Python (Pandas) – Data cleaning and exploratory analysis
    
    Power BI – Data visualization and dashboards
    
    Excel – Data inspection and preprocessing

📊 Key KPIs & Metrics
📦 Inventory Metrics

    1) Inventory Turnover Ratio
    
    2) Understock & Overstock Products
    
    3) Stock Status (Understock / Optimal / Overstock)



🚚 Supply Chain Metrics
    
    1) On-Time Delivery Percentage
    
    2) Average Delivery Delay
    
    3) Warehouse-wise Performance
    
    4) Region-wise Order Distribution

🏭 Supplier Metrics

    1) Average Lead Time
    
    2) Supplier Rating
    
    3) Supplier Performance Score
    
    4) Delay Impact by Supplier

🧮 SQL Analysis

    1) SQL was used to perform:
    
    2) Data joins across multiple tables
    
    3) Aggregations using GROUP BY
    
    4) Conditional logic using CASE
    
    5) KPI calculations for supply chain performance

Example SQL query:

SELECT 
    ROUND(100.0 * SUM(CASE WHEN delivery_date <= expected_delivery_date THEN 1 ELSE 0 END) / COUNT(*), 2) 
    AS on_time_delivery_percentage
FROM orders;

📈 Power BI Dashboard

The Power BI report consists of four main pages:

1️⃣ Executive Overview

Total Orders

    1) Total Revenue
    
    2) On-Time Delivery %
    
    3) Inventory Turnover
    
    4) Sales and order trends

2️⃣ Inventory Analysis

    1) Stock levels by product and warehouse
    
    2) Understock and overstock analysis
    
    3) Category-wise inventory distribution

3️⃣ Warehouse Performance

    1) Average delivery delay by warehouse
    
    2) Orders by warehouse
    
    3) Delay trends over time

4️⃣ Supplier Performance

    1) Lead time by supplier
    
    2) Supplier rating vs lead time (scatter plot)
    
    3) Supplier performance table


💡 Key Insights

    1) Certain products frequently fall below reorder levels, increasing stockout risk.
    
    2) Some warehouses consistently show higher delivery delays.
    
    3) Suppliers with longer lead times negatively impact order fulfillment.
    
    4) Overstocked products contribute to higher inventory holding costs.
    
    5) Supplier ratings do not always align with actual delivery performance.

📌 Business Impact

This project demonstrates how data analytics can:

    1) Optimize inventory management
    
    2) Improve supplier selection and monitoring
    
    3) Reduce delivery delays
    
    4) Minimize lost sales

    5) Support strategic supply chain decisions

🚀 Future Enhancements

    1) Demand forecasting using machine learning
    
    2) Real-time dashboard integration
    
    3) Cost optimization analysis
    
    4) Predictive supply chain modeling

👤 Author

Rishi Bhardwaj
Aspiring Data Analyst

Skills: SQL | Python | Power BI | Excel | Data Analysis

linkedin - www.linkedin.com/in/rishi-b-93b91b296
