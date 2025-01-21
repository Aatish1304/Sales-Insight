
# SALES Insight

A brief description of what this project does and who it's for
Dashboard Link : https://app.powerbi.com/links/wbtJngxyza?ctid=a3da1a5e-6af9-42be-8ad1-2a9b41101b90&pbi_source=linkShare

Problem Statement

This dashboard helps businesses understand their sales performance better. It provides insights into customer behavior, sales trends, and product performance. By analyzing key metrics, businesses can identify areas of improvement and enhance their strategies to boost sales and customer satisfaction.

The dashboard reveals that certain products and regions underperform, while others excel. By identifying these trends, businesses can focus on problem areas and replicate successful strategies elsewhere.

Steps Followed

Step 1: Load data into Power BI Desktop, dataset is a CSV file.

Step 2: Open Power Query Editor and, under the "View" tab in the "Data Preview" section, check "Column Distribution," "Column Quality," and "Column Profile" options.

Step 3: Since profiling is by default limited to 1000 rows, select "Column Profiling Based on Entire Dataset."

Step 4: Identify and handle null values. For instance, the "Sales" column had some missing data, which was excluded from calculations as it comprised less than 1% of the dataset.

Step 5: Select a theme in the "Report View" for consistent design.

Step 6: Add visuals to represent various metrics, such as sales trends, product performance, and customer demographics, using the visualizations pane.

Step 7: Use slicers for key fields, such as "Region," "Product Category," and "Customer Type."

Step 8: Create card visuals to display key metrics, such as total sales, average order value, and total number of transactions.

Null values were excluded from average calculations using visual-level filters.

Step 9: Add a bar chart to visualize sales by product category, segmented by region.

Step 10: Create measures and calculated columns to enhance data analysis:

Calculated Column: Segment customers into different spending categories using the following DAX expression:

Spending Category =
IF(sales_data[Total Spend] <= 100, "Low Spender",
IF(sales_data[Total Spend] <= 500, "Medium Spender",
"High Spender"))

Step 11: Add KPI cards to highlight:

Total Revenue

Revenue Growth Percentage

Profit Margin

Step 12: Use stacked bar charts and pie charts for visual representation of:

Sales distribution by region

Product categories contributing to revenue

Customer demographics, such as age groups and spending behavior

Step 13: Add text boxes and shapes for dashboard titles, subtitles, and highlighting specific insights.

Step 14: Publish the report to Power BI Service for collaboration and sharing.

Insights

Key takeaways from the Sales Insight Dashboard:

Total Sales: $X (adjusted dynamically with slicers)

Top Performing Region: Region A with $Y in sales

Underperforming Region: Region B with $Z in sales

Product Performance:

Best-selling category: Electronics

Least-performing category: Furniture

Customer Segments:

High Spenders: 20%

Medium Spenders: 50%

Low Spenders: 30%

Demographic Trends:

Majority of customers are aged 25-45 years.

High spenders predominantly fall in the 35-45 age group.

Average Order Value: $XX

Recommendations

Focus marketing efforts on underperforming regions.

Expand the product range in best-performing categories.

Improve promotions and discounts for low-performing products.

Analyze customer feedback to enhance customer experience and satisfaction.

Next Steps

Implement advanced analytics, such as predictive modeling, to forecast future sales trends.

Integrate real-time data feeds for up-to-date insights.

Enhance the dashboard with more interactive visuals, such as drill-through reports and what-if analyses.


