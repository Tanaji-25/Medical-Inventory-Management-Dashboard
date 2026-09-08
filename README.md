💊 Medical Inventory Management Dashboard

An interactive Power BI dashboard designed to provide a consolidated view of medical sales, inventory movement, profitability, and product return risks. The dashboard helps management quickly identify revenue drivers, monitor financial performance, and analyze inventory-related risks.

📊 Recommended Structure and Order
1. Project Title / Headline
💊 MedCure Medical Inventory & Sales Analytics Dashboard

An interactive Power BI business intelligence solution for analyzing medical product sales, inventory movement, profitability, returns, departments, and high-performing medicines.

The dashboard transforms raw medical transaction data into actionable insights for management and decision-making.

2. Short Description / Purpose

The MedCure Medical Inventory Management Dashboard is an interactive Power BI report developed to provide management with a consolidated view of the organization's sales performance, costs, profitability, product movement, and return-related inventory risks.

The dashboard enables users to quickly identify top-selling medicines, high-contributing departments, sales trends, profitability, and monthly return rates through interactive KPIs, charts, and filters.

Business Problem

MedCure's sales and inventory data contains valuable information across medicines, departments, dates, costs, sales, and returns. However, analyzing these metrics individually can make it difficult for management to quickly understand overall financial performance and identify potential inventory risks.

Goal

The goal of this dashboard is to provide a single interactive management view that helps answer:

How are sales performing over time?
Which medicines generate the highest revenue?
How much profit is being generated?
What is the overall gross margin?
Which departments contribute the most sales?
What is the financial impact of returned products?
Are return rates increasing or decreasing over time?
3. Tech Stack

The dashboard was developed using the following tools and technologies:

📊 Power BI Desktop – Main business intelligence and data visualization platform.
📂 Power Query – Used for data preparation, transformation, and validation.
🧠 DAX (Data Analysis Expressions) – Used to create business measures and KPIs such as Net Sales, Gross Profit, Gross Margin %, and Return Rate.
🗂️ Data Modeling – Created relationships between the transaction table and a dedicated Calendar table for time-based analysis.
📅 Date/Time Intelligence – Used for monthly, quarterly, yearly, and trend analysis.
📈 Interactive Visualizations – KPI cards, line charts, bar charts, donut charts, slicers, and interactive filtering.
📁 Microsoft Excel – Source data format.
📄 File Format – .pbix for the Power BI report and .xlsx for the source dataset.
4. Data Source
Source

The dashboard was created using a cleaned medical inventory and sales dataset provided in Excel format.

The dataset contains transaction-level information related to medical products, sales, costs, returns, patients, departments, and product classifications.

Key Data Fields

The dataset includes fields such as:

Category	Fields
📅 Date	Dateofbill, Month, Year, Day
💊 Product	DrugName, Formulation, SubCat, SubCat1
🏥 Department	Dept, Specialisation
👤 Patient	Patient_ID
📦 Inventory	Quantity, ReturnQuantity
💰 Financial	Final_Sales, Final_Cost, RtnMRP
📈 Performance	Profit, Profit_margin, Sales_per_Unit
🔄 Transaction	Typeofsales

The data was prepared and structured in Power Query before being modeled and visualized in Power BI.

5. Features / Highlights
🔹 Business Problem

Medical organizations need to continuously monitor product sales, profitability, inventory movement, and returns. However, analyzing these metrics from raw transaction data can make it difficult to identify important trends and risks quickly.

For example:

Which medicines are the biggest revenue generators?
Which departments contribute the most sales?
Is profitability improving?
How significant are product returns?
Are return rates increasing in certain months?
How is overall sales performance changing over time?

This dashboard addresses these questions through an interactive executive reporting solution.

🎯 Goal of the Dashboard

The dashboard was designed to:

Provide management with a consolidated view of financial performance.
Monitor sales and cost trends.
Identify high-value medicines.
Analyze department-level sales contribution.
Monitor product return value and return rates.
Track profitability and gross margin.
Allow users to interactively filter results by year, month, department, drug, and other dimensions.
📌 Walkthrough of Key Visuals
💰 Key Performance Indicators

The executive dashboard provides high-level KPIs for quick management review:

Total Net Sales – Revenue after accounting for returned product value.
Gross Margin % – Measures profitability relative to total sales.
Total Return Value – Financial value of returned products.
Return Rate (Value) – Percentage of sales value associated with returns.

These KPIs allow management to quickly assess the overall financial health and inventory-related risk.

📈 Sales Trend

A monthly sales trend visual shows how Final Sales have changed over time.

This helps identify:

Growth or decline in sales
Monthly fluctuations
Potential seasonality
High-performing periods
Periods requiring further investigation
💵 Sales vs Cost

A combined Sales vs Cost visualization compares:

Final Sales

against

Final Cost

over time.

This helps management understand whether increasing sales are translating into improved profitability.

💊 Top 10 Selling Medicines

A Top 10 DrugName visualization ranks medicines based on Final Sales value.

This identifies the organization's highest-value products and helps management understand which medicines are major contributors to overall revenue.

🔄 Return Ratio

The dashboard tracks the Return Rate (Value) on a monthly basis.

This metric is calculated as:

Return Rate =
Total Return Value / Total Sales

A higher return ratio can indicate potential inventory, product, operational, or customer-related issues requiring further investigation.

🏥 Department Contribution

A department-level visualization compares sales contribution across different departments.

This helps answer:

Which departments contribute the most to overall sales?

It can be used to identify high-performing departments and compare their relative contribution to the organization's revenue.

🎛️ Interactive Filters

The dashboard includes interactive slicers that allow users to analyze the data dynamically by:

Year
Quarter
Month
Department
Drug Name
Formulation
Specialisation

When a filter is selected, the KPIs and charts automatically update to reflect the selected context.

🧮 DAX Measures

The dashboard uses DAX measures to calculate important business KPIs.

Total Sales
Total Sales =
SUM('Table'[Final_Sales])
Total Cost
Total Cost =
SUM('Table'[Final_Cost])
Total Return Value
Total Rtn MRP =
SUM('Table'[RtnMRP])
Total Net Sales
Total Net Sales =
[Total Sales] - [Total Rtn MRP]
Gross Profit
Gross Profit =
[Total Sales] - [Total Cost]
Gross Margin %
Gross Margin % =
DIVIDE([Gross Profit], [Total Sales], 0)
Return Rate
Return Rate (Value) =
DIVIDE([Total Rtn MRP], [Total Sales], 0)
📊 Data Model

A dedicated Calendar table was created to support time-based analysis.

The Calendar table was related to the transaction table using:

Calendar[Date]
       │
       │ 1 : *
       ▼
Table[Dateofbill]

This enables consistent analysis across:

Year
Quarter
Month
Date
Sales trends
Return trends
Profitability trends
💡 Business Impact & Insights
Revenue Optimization

The Top 10 medicine analysis helps identify products that generate the highest sales value, allowing management to focus on high-value products.

Inventory Risk Monitoring

Return Value and Return Rate provide a high-level indicator of products that may require additional investigation.

Profitability Management

Gross Profit and Gross Margin allow management to evaluate whether sales growth is translating into healthy financial performance.

Department Performance

Department-level analysis helps identify the areas contributing most significantly to overall revenue.

Trend & Seasonality Analysis

Monthly sales trends help management identify fluctuations and potential seasonal patterns that can support future planning.

Data-Driven Decision Making

The dashboard converts transaction-level medical data into an interactive management reporting solution, reducing the need for manual analysis.

6. Screenshots / Demos
