# CEO-s-Coffeeshopanalysis
Provides a structured summary of the analytical work conducted for the coffee shop, utilizing SQL for data extraction and manipulation, and Microsoft Excel for in-depth analysis and visualization

Project Overview
This project leverages historical transactional data from Bright Coffee Shop to generate business insights for the newly appointed CEO. The goal is to identify opportunities for revenue growth and operational improvement through data-driven decision-making.

Objective
Use SQL and data visualization tools to:
- Determine top revenue-generating products
- Analyze peak sales periods throughout the day
- Identify product and time-based sales trends
- Provide actionable recommendations to boost performance

Tools & Technologies
- SQL Engines: Snowflake, Microsoft SQL Server
- Visualization Platforms: Microsoft Excel
- Planning: Miro
- Presentation: Canva

Tasks Breakdown
1. Planning & Architecture (Miro)
- Data Flow Design:
  - Source: Excel transactional dataset
  - Processing: ETL pipeline using Snowflake
  - Storage: Snowflake cloud data warehouse
  - Output: Visualizations and dashboards
- Key Insights Outlined:
  - Revenue by product and time bucket
  - High vs. low-performing product SKUs
  - Total units and total revenue metrics
- Calculated Fields:
  - `total amount = unit price * transaction_qty`
  - Grouping by 30-minute or hourly intervals

2. Data Transformation (SQL/Snowflake)
- Converted Excel data to CSV and loaded into Snowflake
- Cleaned and transformed data:
  - Handled inconsistent numeric formats (e.g. '3,1' → 3.1)
  - Created `transaction_time_bucket` column
  - Aggregated sales by product, time, and quantity
- SQL queries saved in `sql/bright_coffee_analysis.sql`

3. Excel Data Analysis & Visualization
- Exported cleaned data from Snowflake into Excel
- Created dynamic pivot tables for:
  - Sales trends by product and time
  - Total revenue and quantity sold
  - Product performance comparisons
- Developed visuals using bar graphs, line charts, and pie charts

4. CEO Presentation (PowerPoint)
- Methodology: Project workflow, data sources, and logic used
- Insights: Sales trends and revenue breakdown
- Recommendations:
  - Introduce promos during off-peak times
  - Prioritize stocking top-selling items
  - Encourage sales of underperforming products
- Next Steps:
  - Automate future sales reporting
  - Plan for multi-location analytics
  - Launch loyalty incentives for peak customers

