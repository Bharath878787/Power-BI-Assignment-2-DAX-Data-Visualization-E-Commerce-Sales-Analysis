# Power-BI-Assignment-2-DAX-Data-Visualization-E-Commerce-Sales-Analysis
This repository showcases my Power BI project on E‑Commerce Sales Analysis, where I applied Power Query transformations, DAX calculations, and interactive data visualizations to analyze sales performance, targets, and profitability.

Calculated Columns:
1. Create a Calculated Column for 'Category Type': Add a calculated column in the Order Details table that combines the 'Category' and 'Sub-Category' columns into a
single 'Category Type' column.
Answer : I Have created a calculated column named Category Type and used "&" to merge Category and Sub-category and used "-" as Delimiter.

2. Calculate Revenue per Order in Order Details Table: Create a calculated column in the Order Details table to compute the revenue (Amount * Quantity) per order.
Answer : I Created a New Column Named "Revenue per order" and multiplied Amount and Quantity using "*" Operator.

3.Create a Calculated Column to Categorize Sales: Add a calculated column named ‘Sales Category’ in the Order Details table that categorizes each order as 'Above
Average' or 'Below  Average' based on the Amount value.
Answer : I created a New Column named "Sales Category" and categorized each order as 'Above Average' or 'Below  Average' based on the Average Amount value.


Calculated Measures:
4. Calculate Order Count: Define a measure to count the total number of orders in the Order Details table.
Answer : Created a New Measure named "Total no. of Orders" in Order Details Table and used COUNTROWS DAX function to calculate the total Orders.

5. Calculate Average Profit in Delhi: Create a measure to calculate the average profit for orders placed in Delhi.
Answer : I have created a new Measure named Average profit in Delhi using Calculate and Filter DAX Functions in the "Orders Data" Table.

6. Calculate Year-to-Date (YTD) Sales: Define a measure to calculate the total sales amount accumulated from the earliest order date up to each order date.
Answer : I have created a New Measure name YTD Sales and used TOTALYTD DAX Function.

Data Visualization:
7. Sales Target Achievement by Category: Compare actual sales with sales targets by category using a clustered column chart.
Answer : I have created a Clustered Column chart and dragged category column into x-axis and sum of amount from order Details Table and sum of target in y-axis from Sales Target Table.

8. Max Profit Margin by Sub-Category: Analyze the maximum profit margin for each sub-category of products using a donut chart.
Answer : I have created a new table by using group by function for sub-category column and used max operation to profit margin column and inserted donut chart and  dragged max of profit margin in values and Sub-Category in Legend from Max Profit Margin by Sub-Category Table.

9. Monthly Sales Trend: Show the trend of monthly sales over time using a line chart.
Answer : I have inserted Line Chart dragged Order Date in x-Axis and Sum of Amount in y-axis from Orders Data Table.

10. Comparison of Profit and Quantity by Sub-Category: Compare the relationship between profit and quantity sold for different sub-categories using a scatter chart.
Answer : I have inserted Scatter chart dragged sub-category into Legend, Sum of Quantity into x-axis and Sum of Profit into Y-Axis from Order Details table.

11. Comparison of Total Sales Amount and Target: Create cards to succinctly display the total sales amount alongside the sales target for quick comparison and analysis. Also, create a multi-row card to display the minimum target for each segment.
Answer : I have created cards used sum of amount column from Order Details Table and sum of Target from Sales Target Table into another Card . I didn't find multi row card in my Visualizations.

12. Sales Performance Matrix: Build a matrix view to analyze how actual sales compare to sales targets across different categories and months.
Answer : I have inserted matrix dragged order date in Rows , Category in Columns , sum of Amount columns from Order Details Table and Sum of Target column from Sales Target table into Values.

13. Geographic Sales Analysis: Visualize total sales on a map by city to identify regional sales patterns.
Answer : I inserted Map dragged Location Column into Location and Sum of Amount column in Bubble Size from Orders Data Table.

14. Sales Distribution by Sub-Category: Represent the sales distribution across different sub-categories using a tree map.
Answer : I inserted Tree map dragged Sub-category column into Category and Sum of Amount column into Values from Orders Data Table. 

15. Order Count Analysis by State: Create a funnel chart to visualize the distribution of order counts across different states.
Answer : I inserted Funnel Chart dragged Location Column into Category and count of order ID Column into Values from Orders Data Table.
