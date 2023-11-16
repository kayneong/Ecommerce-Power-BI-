# Ecommerce-Power-BI-

# Project Title
PowerBI Sales Dashboard for a US Based Ecommerce Company

# Project Overview 
The goal of this project is to create a sales dashboard showing information on Year-to-Date (YTD) Sales and generate insights for the scenarios below: 
 - KPI banner showing YTD Sales, Profit, Quantity sold, Profit Margin
 - Year-on-year (YoY) growth for each KPI and YTD sparkline for each measure in the KPI to understand the monthly trend
 - Find YTD Sales, Past-Year-to-Date (PYTD) Sales, and YoY Sales growth for different customer categories. Adding a trend icon for each category
 - Find YTD Sales performance by each state
 - Top 5 and Bottom 5 products by sales
 - YTD Sales by region to know the best and worst performing regions all over the US
 - YTD Sales by shipping type to get the highest sales percentage shipping type

# Business Understanding 
A sales dashboard is a crucial visual representation of the company's performance metrics. It gives a concise view of results-based data and helps sales and marketing managers identify opportunities to make changes and increase revenue for the company. It allows identification of who the best customers are, where the challenges lie, and what changes may be needed to increase sales. It can also help with forecasting future revenue. 

# Data Understanding 
This dashboard has been built upon two separate datasets which are attached in this repository. 'ecommerce_data' and 'us_state_long_lat_codes'. The ecommerce_data contains 113271 rows and 21 columns with each row representing each customer that has made a purchase and each column representing various features like the product name, customer segment, state of the customer, customer name, and more. The dataset has been cleaned and there are no missing values or duplicates remaining. The .csv file was loaded into an SQLExpress server with the type of columns identified as nvar50 changed to var50 while the 'product_name' column was changed to var200 to fit the longer text length of the product names. The e-commerce dataset's 'customer_state' column was also mapped to the us_state_long_lat_codes dataset's 'name' column to establish a relationship between the two datasets. Furthermore, a Calendar table was constructed for the usage of time intelligence functions. The 'Date' column of the Calendar table was subsequently mapped to the 'order_date' of the ecommerce_data dataset as well. 

# Dashboard Preview
The dynamic and interactive dashboard below was built on Power BI Desktop and allows a concise and informative view of various KPIs, sales-related tables, and graphs. It also allows filtering by customer segments, states, and regions. 

 ![image](https://github.com/kayneong/Ecommerce-Power-BI-/assets/150570357/a2834d0d-4f88-4424-a749-e99671eeabe5)

 # Conclusion
This project has been completed successfully as part of a learning portfolio project to practice building interactive dashboards on PowerBI as a beginner. The key learning takeaways for this project were:
 - How to connect PowerBI to MS SQL server and flat files
 - Data modeling with three tables
 - Data cleaning in Power Query
 - How to create a data table in Power BI (Calendar table)
 - Time intelligence functions (TOTALYTD, SAMEPERIODLASTYEAR, etc)
 - Creating dynamic and complex KPIs
 - Basic to Advanced Dax Queries (Calculate, Sum, concatenate, var)
 - Conditional Formatting, Adding dynamic icons in Power BI
 - Creating different charts, maps and formatting them
 - Generating insights from charts
