# Power-BI-Assignment-2-DAX-Data-Visualization-E-Commerce-Sales-Analysis
This repository showcases my Power BI project on E‑Commerce Sales Analysis, where I applied Power Query transformations, DAX calculations, and interactive data visualizations to analyze sales performance, targets, and profitability.

## 📌 Calculated Columns
**Q1. Create a Calculated Column for 'Category Type'**  
Add a calculated column in the Order Details table that combines the 'Category' and 'Sub-Category' columns into a single 'Category Type' column.  
**Answer:** I created a calculated column named *Category Type* and used `&` to merge Category and Sub-Category with "-" as delimiter.

**Q2. Calculate Revenue per Order in Order Details Table**  
Create a calculated column in the Order Details table to compute the revenue (Amount * Quantity) per order.  
**Answer:** I created a new column named *Revenue per Order* and multiplied Amount and Quantity using the `*` operator.

**Q3. Create a Calculated Column to Categorize Sales**  
Add a calculated column named ‘Sales Category’ in the Order Details table that categorizes each order as 'Above Average' or 'Below Average' based on the Amount value.  
**Answer:** I created a new column named *Sales Category* and categorized each order as 'Above Average' or 'Below Average' based on the Average Amount value.

---

## 📌 Calculated Measures
**Q4. Calculate Order Count**  
Define a measure to count the total number of orders in the Order Details table.  
**Answer:** I created a measure named *Total no. of Orders* using the `COUNTROWS` DAX function.

**Q5. Calculate Average Profit in Delhi**  
Create a measure to calculate the average profit for orders placed in Delhi.  
**Answer:** I created a measure named *Average Profit in Delhi* using `CALCULATE` and `FILTER` functions.

**Q6. Calculate Year-to-Date (YTD) Sales**  
Define a measure to calculate the total sales amount accumulated from the earliest order date up to each order date.  
**Answer:** I created a measure named *YTD Sales* using the `TOTALYTD` function.

---

## 📊 Data Visualizations
**Q7. Sales Target Achievement by Category**  
Compare actual sales with sales targets by category using a clustered column chart.  
**Answer:** I created a Clustered Column chart with Category on X-axis, Sum of Amount (Order Details) and Sum of Target (Sales Target) on Y-axis.

**Q8. Max Profit Margin by Sub-Category**  
Analyze the maximum profit margin for each sub-category using a donut chart.  
**Answer:** I created a grouped table by Sub-Category with MAX of Profit Margin, then used Sub-Category in Legend and Max Profit Margin in Values in a Donut chart.

**Q9. Monthly Sales Trend**  
Show the trend of monthly sales over time using a line chart.  
**Answer:** I inserted a Line Chart with Order Date on X-axis and Sum of Amount on Y-axis.

**Q10. Profit vs Quantity by Sub-Category**  
Compare profit and quantity sold for different sub-categories using a scatter chart.  
**Answer:** I inserted a Scatter Chart with Sub-Category in Legend, Sum of Quantity on X-axis, and Sum of Profit on Y-axis.

**Q11. Total Sales Amount vs Target**  
Create cards to display total sales amount and sales target. Also, create a multi-row card to display minimum target per segment.  
**Answer:** I created cards with Sum of Amount and Sum of Target. I couldn’t find the Multi-Row Card visualization.

**Q12. Sales Performance Matrix**  
Build a matrix view to analyze how actual sales compare to sales targets across categories and months.  
**Answer:** I inserted a Matrix with Order Date in Rows, Category in Columns, and Sum of Amount + Sum of Target in Values.

**Q13. Geographic Sales Analysis**  
Visualize total sales on a map by city.  
**Answer:** I inserted a Map with Location in Location field and Sum of Amount in Bubble Size.

**Q14. Sales Distribution by Sub-Category**  
Represent sales distribution across sub-categories using a treemap.  
**Answer:** I inserted a Treemap with Sub-Category in Group and Sum of Amount in Values.

**Q15. Order Count Analysis by State**  
Create a funnel chart to visualize distribution of order counts across states.  
**Answer:** I inserted a Funnel Chart with Location in Category and Count of Order ID in Values.
