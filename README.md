# Coffee-Shop-Sales-analysis-with-SQL-and-Power-BI
Data Transformation:

Date and Time Conversion: The transaction_date and transaction_time columns are converted to proper date and time formats using the STR_TO_DATE() function, ensuring consistency and accuracy. Afterward, the columns are modified to DATE and TIME data types, respectively, for better handling of date-related operations.
Column Name Correction: The column ï»¿transaction_id is renamed to transaction_id to remove any unwanted characters caused by encoding issues.
Sales Analysis:

Total Sales Calculation: A query calculates the total sales for May by multiplying the unit price with the quantity sold (unit_price * transaction_qty), summing the result, and rounding it to the nearest integer.
Sales Growth (MoM): The LAG() function is used to calculate the month-over-month (MoM) sales growth, allowing the comparison of sales figures between consecutive months. This is expressed as a percentage increase or decrease.
Orders and Quantity Sold:

Total Orders: A query calculates the total number of orders (transactions) for May by counting the transaction_id.
Total Quantity Sold: This query sums up the quantities of products sold in May, providing an overview of product demand.
Sales Trends and Comparison:

Daily Sales Trend: A query groups the data by day and calculates the sales for each day in May, helping identify daily trends and fluctuations.
Comparison with Average Sales: Daily sales are compared to the average sales for May to determine whether each day’s sales are above, below, or at average levels.
Sales by Weekday/Weekend: The sales are categorized into weekdays and weekends using DAYOFWEEK() to determine patterns of sales based on customer behavior during different days of the week.
Sales by Category and Location:

Sales by Product Category: The query provides a breakdown of sales by product category, helping to identify which types of products are driving revenue.
Sales by Store Location: This query calculates sales by store location, identifying which stores perform better in terms of sales.
Sales by Hour and Day:

Sales by Hour: An analysis of sales is carried out based on different hours of the day, identifying peak sales times for better staffing and operational planning.
Sales by Day of Week: The query groups sales by day of the week to compare performance from Monday to Sunday, offering insights into the weekly sales patterns.
Conclusion:
These queries offer a comprehensive analysis of the coffee shop’s sales data, enabling better decision-making based on daily, weekly, and monthly trends. By transforming the data into the right formats, calculating key performance indicators (KPIs), and breaking down sales by various factors such as time, product, and location, the business can gain valuable insights to optimize operations, marketing strategies, and customer engagement.
