## Pharma Analytics Project

# Business Context

Hospitals depend on timely delivery of medical products (implants, kits, consumables) to support patient care 
and surgical procedures. Delays, cancellations, or poor demand visibility can directly impact hospital operations 
and clinical outcomes.

This project simulates a MedTech / Pharma supply chain analytics use case, focusing on 
how hospital orders translate into product revenue and how operational performance (warehouses and logistics) 
affects service reliability.

The dashboard is designed from the perspective of a Senior Data Analyst supporting Operations and Analytics teams

-----------------------------------------------------------------------------------------------------

# Objectives

- Analyze hospital order patterns and demand behavior
- Track product-level revenue and clinical usage signals
- Evaluate warehouse and shipment performance, with focus on delays
- Enable management-level visibility through interactive dashboards

-----------------------------------------------------------------------------------------------------

# Data Overview

The project uses structured CSV datasets representing:

- Orders: Hospital purchase requests for medical products
- Products: Product master data with pricing
- Hospitals: Customer entities placing orders
- Warehouses: Fulfillment locations
- Shipments: Delivery status and logistics performance
- Dates: Calendar dimension for time-based analysis

These datasets together form an end-to-end hospital supply chain view.

-----------------------------------------------------------------------------------------------------

# Data Architecture

Bronze → Silver → Gold approach
Bronze: Raw CSV data ingested into Snowflake
Gold: Aggregated business-ready tables in Snowflake for analytics and dashboards
Snowflake is used as the analytical data warehouse, connected directly to Power BI for reporting.
Files were imported in Power BI for further analysis

-----------------------------------------------------------------------------------------------------

# Key Metrics & KPIs

- Hospital Order Metrics
  Total Orders
  Delayed Orders
  Order Trends (Monthly)

- Revenue Metrics
    Total Revenue
    Revenue by Product
    Revenue by Hospital
    Revenue Trends Over Time

- Operations & Logistics Metrics
    Delayed Shipments
    Average Delayed Shipments per Warehouse
    Warehouse-level Operational Comparison

-----------------------------------------------------------------------------------------------------
# Key Insights

- Hospital orders represent time-critical clinical demand, making delivery reliability a key performance driver
- High-revenue products are typically associated with frequent or critical medical procedures.
- Shipment delays are uniform across warehouses, indicating systemic or upstream constraints rather than warehouse-specific issues.

-----------------------------------------------------------------------------------------------------

# Tools & Technologies

- Snowflake: Cloud data warehouse and SQL analytics
- SQL: Data modeling, transformations, aggregations
- Power BI: Interactive dashboards and data visualization
- Star Schema Modeling: Fact and dimension design for analytics

-----------------------------------------------------------------------------------------------------

# Dashboard Highlights

- Executive-level KPI cards for Orders, Revenue, and Delays
- Monthly trend analysis with drill-downs
- Warehouse comparison for logistics performance
- Product revenue ranking to identify key drivers

The dashboard is designed for Operations Leadership and Analytics Teams to support decision-making.

-----------------------------------------------------------------------------------------------------

# Business Value

- Improves visibility into hospital demand and fulfillment performance
- Helps identify operational risks impacting patient care
- Enables data-driven discussions between operations, logistics, and commercial teams

-----------------------------------------------------------------------------------------------------

# Author Notes

This project demonstrates end-to-end analytics skills including:
- Business problem understanding
- Data modeling and SQL proficiency
- BI dashboard design and storytelling
- Healthcare / MedTech domain alignment
- Utilizing modern cloud data tools like Snowflake

-----------------------------------------------------------------------------------------------------

# DashBoard Preview

### Executive Summary
![Executive Summary](dashboard_images/01_Executive_Summary.png)

### Product Revenue Analysis
![Product Revenue](dashboard_images/03_Product_Revenue.png)

### Warehouse & Shipment Performance
![Warehouse Delays](dashboard_images/04_Warehouse_Delays.png)
