# 📊 Sales Performance Analytics Dashboard

![Power BI](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=Power%20BI&logoColor=black)
![Data Analytics](https://img.shields.io/badge/Data_Analytics-1E88E5?style=for-the-badge&logo=data&logoColor=white)

## 📌 Project Overview
A comprehensive Power BI Business Intelligence solution designed to track, analyze, and visualize overall sales performance, product profitability, and employee contributions. This project transforms raw operational data into actionable business insights.

## 🎯 Business Problem
The management team lacked a centralized view of sales performance across different regions and product categories. Tracking individual employee performance and identifying high-margin products was a manual and time-consuming process, leading to delayed decision-making.

## 💡 Business Objectives
- **Sales Tracking:** Monitor revenue and profit trends over multiple years.
- **Product Performance:** Identify top-performing and underperforming product categories.
- **Employee Evaluation:** Analyze individual sales contributions to recognize top performers.
- **Geographic Insights:** Visualize sales distribution across different countries.

## 🗄️ Dataset
- **Orders:** Transactional data including OrderID, CustomerID, OrderDate, Sales, and Profit.
- **Product Details:** Information on Categories, Products, and Suppliers.
- **Employee:** Demographics and organizational data of the sales team.

## 🛠️ Tech Stack
- **Data Visualization & BI:** Power BI
- **Data Transformation:** Power Query
- **Data Modeling:** Star Schema (1-to-Many Relationships)
- **Calculations:** DAX (Data Analysis Expressions)

## 🚀 Dashboard Preview

### Executive Overview
*(Provides a high-level summary of key performance indicators, sales by category, yearly trends, top employees, and geographical sales distribution.)*

![Executive Overview](screenshots/01-executive-overview.png)

## 🏗️ Data Model
The project utilizes a **Star Schema** to optimize query performance and ensure accurate filtering across visualizations.

![Data Model](screenshots/02-data-model.png)

## ⚙️ Power Query & Data Cleaning
- Changed data types for accuracy (e.g., Dates, Currencies, Text).
- Handled missing values and standardized text formats.
- Created relationships based on primary and foreign keys.

## 🧮 DAX Measures
Implemented core DAX measures to drive the KPI cards and visuals. Examples include:
- `Sum of Sales = SUM(Orders[Sales])`
- `Sum of Profit = SUM(Orders[Profit])`

## 📊 Business Insights
1. **Sales Growth:** Clear upward or downward trends can be identified via the Year-over-Year chart.
2. **Top Categories:** Specific product categories consistently drive the majority of the profit margin.
3. **Key Performers:** A small percentage of the sales team is responsible for a large portion of total revenue.

## 🔮 Future Improvements
- Implement Row-Level Security (RLS) so managers only see their respective regional data.
- Add dynamic Time Intelligence measures (YTD, MTD, YoY%).
- Include predictive analytics for next quarter's sales forecasting.

## 💼 Skills Demonstrated
- Business Intelligence & Dashboard Design
- Relational Database Concepts (Data Modeling)
- ETL Processes (Extract, Transform, Load)
- Data Storytelling

---
**Contact:** [Your Name/LinkedIn/Email]