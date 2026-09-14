Project Overview
This project focuses on evaluating e-commerce sales performance and customer behavior. The goal of this analysis is to identify key sales trends, customer segmentation, and product performance using SQL for data extraction and cleaning, followed by Tableau for interactive data visualization.
publish


🎯 Business Problem & Objective
The management team needed a way to track Key Performance Indicators (KPIs) regarding sales, profit, and customer retention.

Objectives:

Clean and format raw sales data for analysis.
Identify the highest-grossing product categories and seasonal sales trends.
Determine customer purchase frequency and segment high-value customers.
Build an interactive dashboard for stakeholders to filter data dynamically by year, region, and product type.
🛠️ Tools & Technologies Used
SQL (MySQL / PostgreSQL / SQL Server): Used for Data Cleaning, Exploratory Data Analysis (EDA), Aggregations, Window Functions, and CTEs.
Tableau: Used for connecting the database, creating calculated fields, and building an interactive dashboard layout.
Excel / CSV: Initial raw dataset formats before database importing.
🗂️ Data Preparation & SQL Exploration
The raw data contained inconsistencies, null values, and formatting errors. I used SQL to clean the data and perform exploratory analysis.

Key SQL Skills Demonstrated:

Creating tables and importing data constraints.
Handling Null values and duplicate records.
Using JOIN to combine Customer and Sales tables.
Utilizing CTEs (Common Table Expressions) and Window Functions (e.g., RANK(), PARTITION BY) to find top-selling items per region.
Date manipulation (EXTRACT, DATE_TRUNC) for time-series forecasting.
(You can view the full SQL script in the sql_queries.sql file in this repository).

📈 Tableau Dashboard Development
After exporting the cleaned datasets from SQL, I connected them to Tableau to build out visual representations of the data.

Key Dashboard Features:

Executive KPI Banner: Total Revenue, Total Profit, and Profit Margin percentage.
Time-Series Area Chart: Showing month-over-month sales growth.
Geographical Map: Heatmap of sales distribution across different states/regions.
Interactive Filters: Allows the end-user to slice data by Year, Customer Segment, and Product Category.
💡 Key Insights & Recommendations
Seasonal Spikes: Revenue consistently spikes in Q4, specifically in November and December. Recommendation: Increase marketing spend and inventory stock by mid-October.
Underperforming Regions: The Southern region has a high volume of sales but the lowest profit margins due to extreme discounting. Recommendation: Restrict discount usage in this region to improve profitability.
Customer Retention: 20% of customers account for over 60% of total revenue. Recommendation: Implement a targeted loyalty program for these high-value clients.
🚀 How to Run This Project
Clone this repository to your local machine.
Open your preferred SQL client (e.g., MySQL Workbench, pgAdmin) and run the schema_setup.sql script to create the database.
Import the raw_dataset.csv file into the newly created tables.
Run the queries in the analysis_queries.sql file to view the data manipulation steps.
Open the Sales_Dashboard.twbx file in Tableau Desktop to interact with the visualizations.
