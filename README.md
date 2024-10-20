# Comprehensive-Sales-Data-Analysis

## Objective
The objective of this project is to provide the Sales Manager and Sales Representatives with real-time, data-driven insights into internet sales, customer behavior, and product performance. The interactive Power BI dashboard facilitates better decision-making by comparing actual sales against budget targets and identifying opportunities for sales improvement.

## Project Overview
In today's fast-paced business environment, it is essential for sales teams to have a clear and up-to-date overview of sales data. This project involved building a robust data infrastructure that consolidates internet sales data, cleans it, and visualizes key metrics using Power BI. The data is sourced from both SQL Server and Excel files, processed and cleaned using advanced SQL queries, and presented in an interactive Power BI dashboard.

The solution addresses the sales team's need for actionable insights through detailed dashboards that track key performance indicators (KPIs), filter by customers and products, and compare sales against budgets. It also automates data refresh processes, allowing the team to always access the latest information without manual updates.

## Problem Statement
The sales team lacks a consolidated view of their internet sales performance. Sales data is scattered across multiple systems, including SQL Server databases and Excel spreadsheets, which makes it difficult to track trends and customer behaviors. Furthermore, there is no automated way to compare actual sales against budgets, which leads to inefficiencies in sales tracking and reporting.

Challenges identified:
- Inability to easily track top-selling products and customers.
- Difficulty in comparing sales against budgets.
- Lack of automation in updating and refreshing sales data.
- Poor insights into sales trends over time.

## Solution
To solve these problems, the following steps were taken:
1. **Data Restoration and Cleaning**: Sales data was restored from a `.bkp` file in SQL Server, and advanced SQL queries were used to clean the data, removing duplicates and handling missing values.
2. **Data Integration**: Budget data was sourced from an Excel file, and both SQL and Excel data were integrated into Power BI.
3. **Dashboard Development**: An interactive Power BI dashboard was developed to visualize key metrics. It provides filters to slice data by customer and product, and displays KPIs for sales performance against the 2021 budget.


## Features
- **Sales Overview Dashboard**: A Power BI dashboard that provides a real-time overview of internet sales, allowing users to track product and customer performance.
- **Customer and Product Filtering**: Sales Representatives can filter data by individual customers or products to better understand their top sales contributors.
- **Sales vs Budget Tracking**: Sales Managers can track internet sales against the 2021 budget, identifying variances and opportunities for growth.
- **Daily Data Refresh**: The dashboard automatically refreshes sales data once a day, ensuring that the sales team always has access to the most up-to-date data.

## Workflow

### 1. **Restoring and Cleaning Data in SQL Server**
   - The first step was restoring the `.bkp` file containing the sales data into SQL Server using `SQL Server Management Studio (SSMS)`.
   - Once restored, data cleaning was performed to remove duplicates, fill missing values, and ensure data accuracy.

### 2. **Data Integration in Power BI**
   - Data from SQL Server was combined with an Excel file containing the 2021 budget.
   - Power BI's `Data Model` feature was used to create relationships between tables, such as linking products and customers to their corresponding sales records.

### 3. **Dashboard Creation**
   - A Power BI dashboard was created, showing an overview of internet sales, along with specific filters for sales representatives to track customer and product-level performance.
   - The dashboard was enriched with key performance indicators (KPIs) to track sales against the 2021 budget.

### 4. **Automating Data Refresh**
   - A daily data refresh schedule was implemented in Power BI to ensure that the sales data stays current.

## Visualization
The dashboard provides multiple visual insights for both the Sales Manager and Sales Representatives, allowing them to track and monitor sales data in an easy-to-understand, interactive format. The primary components of the dashboard include:

### 1. **Sales Overview Dashboard**:
   - A **line chart** visualizes internet sales trends over time, showing how sales have fluctuated across different periods.
   - **Bar charts** are used to display the top-performing products and customers, highlighting which customers buy the most and which products are selling well.
   - **KPIs** (Key Performance Indicators) are set up to compare actual sales against the 2021 budget, giving a clear indication of whether the sales team is meeting or exceeding expectations.

### 2. **Customer and Product Analysis**:
   - A **slicer** allows Sales Representatives to filter the data by customer or product, enabling them to drill down into the performance of specific segments.
   - The **product sales table** lists detailed sales figures for each product, helping sales representatives identify opportunities for cross-selling or upselling.

### 3. **Sales vs Budget Comparison**:
   - **Gauge charts** and **KPIs** track internet sales against the budget, helping the Sales Manager monitor progress toward sales targets. This visual shows how actual performance aligns with planned sales figures.
   - **Line charts** compare cumulative sales over time against the budget, providing insight into sales velocity and identifying periods of underperformance.

### 4. **Time-Series Analysis**:
   - The dashboard includes a **time-series visualization** showing internet sales trends by month or quarter, making it easier for the Sales Manager to analyze seasonality in customer demand and adjust strategies accordingly.

All visuals are interactive, allowing the sales team to manipulate filters and drill down into specific metrics for deeper insights. The dashboard also refreshes automatically every day, ensuring the data is always up to date.

## Challenges Faced
- **Data Quality Issues**: Cleaning the sales data was challenging due to duplicate records and missing values. SQL queries were carefully crafted to ensure the data was accurate and consistent.
- **Data Integration**: Combining data from different sources (SQL Server and Excel) required precise alignment of fields and data types.
- **Budget Comparison**: Creating KPIs that compared sales data against the budget involved complex DAX (Data Analysis Expressions) formulas within Power BI.

## Technology Stack
- **SQL Server Management Studio (SSMS)**: Used to restore the `.bkp` file and perform data cleaning with advanced SQL queries.
- **Power BI**: Used to develop the dashboard, create relationships between data sets, and visualize sales metrics.
- **Excel**: Source for the 2021 budget data, which was imported into Power BI for budget comparison.
- **DAX (Data Analysis Expressions)**: Used to create complex calculations and KPIs for sales versus budget comparison.

- 
## User Stories
| No | Role               | Request                                  | User Value                                                       | Acceptance Criteria                                                     |
|----|--------------------|------------------------------------------|-------------------------------------------------------------------|-------------------------------------------------------------------------|
| 1  | Sales Manager       | Dashboard overview of internet sales     | To track which customers and products sell the best               | Power BI dashboard that updates sales data once a day                   |
| 2  | Sales Representative| Detailed internet sales per customer     | Can follow up on customers that buy the most                      | Power BI dashboard that allows filtering by customer                    |
| 3  | Sales Representative| Detailed internet sales per product      | Can follow up on top-selling products                             | Power BI dashboard that allows filtering by product                     |
| 4  | Sales Manager       | Sales dashboard with budget comparison   | Track sales over time and compare against the 2021 budget          | Power BI dashboard with KPIs and graphs comparing sales against budget  |

## How to Run the Project

1. **Restoring the `.bkp` file**:
    - Run the `restore_bkp_file.sql` script located in the `SQL/` folder to restore the sales data to SQL Server.
    
2. **Clean and Prepare the Data**:
    - Execute the `data_cleaning.sql` script to remove duplicates and clean the sales data.

3. **Power BI Integration**:
    - Open the Power BI `.pbix` file from the `PowerBI/` folder.
    - Ensure the data sources (SQL Server and Excel) are correctly connected.

4. **Dashboard Visualization**:
    - Load the data and interact with the dashboard to filter by customer, product, and compare against the budget.

## Conclusion
This project provides a solution to streamline sales data analysis for the sales team by automating and visualizing key metrics through Power BI. It integrates data from both SQL Server and Excel to create comprehensive dashboards that provide actionable insights. By automating daily data refresh, the sales team can continuously track performance, improve decision-making, and increase revenue by identifying trends and opportunities.





