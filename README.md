## My-Data-Portfolio-
Collection of projects demonstrating skills in data analysis, visualization, and automation

### Project Title: E-commerce Sales Analysis 

### Project Overview 
This project aims to provide insights into the sales performance of an e-commerce platform by analyzing key metrics such as revenue, customer demographics, sales channels,product categories, seasonal trends, and customer behavior. The analysis helps identify high-performing products, peak sales periods, and customer segments, enabling data-driven decisions to improve sales strategy and customer satisfaction.

### Data Sources
The dataset used in this project is titled [Sales Data.csv ](https://www.kaggle.com), which contains records of sales transactions including details such as product, region, quantity, unit price, order date, customer feedback, sales channels and sales Reps

### Tools Used
- Microsoft Excel
   1. For Data Cleaning 
   2. For Data Analysis 
   3. For Data Visualization 

### Data Cleaning and Preparation 
In the initial phase of data cleaning and preparations, I performed the following actions 
- Data loading and inspection
- Handling missing values
- Data cleaning and formatting

### Exploratory Data Analysis (EDA)
- Total Sales per Product Category
- Sales Transactions in Each Region
- Top Selling Product
- Revenue Per Product
- Monthly Sales for Year 2024
- Top 5 Customers
- Total sales by Day

### Data Analysis 

#### 1. Total Sales per Product Category

- Use a Pivot Table:

-Insert a Pivot Table with "Product Category" as Rows and "Sales Amount" as Values (set to "Sum").

2. Sales Transactions in Each Region

Assuming "Region" is in Column C and "Sales Amount" in Column B.

Use a Pivot Table with "Region" as Rows and "Sales Amount" as Values (set to "Count" or "Sum").

Formula:

=COUNTIF(C2:C100, "Region Name")

Replace "Region Name" with the specific region, C2:C100 with the region column.


3. Top Selling Product

Assuming "Product Name" is in Column D and "Sales Amount" is in Column B.

Use a Pivot Table with "Product Name" as Rows and "Sales Amount" as Values (set to "Sum"). Then sort by the "Sales Amount" column in descending order.

Formula to find the maximum sales:

=INDEX(D2:D100, MATCH(MAX(B2:B100), B2:B100, 0))


4. Revenue Per Product

Use a Pivot Table with "Product Name" as Rows and "Sales Amount" as Values (set to "Sum").

Formula:

=SUMIF(D2:D100, "Product Name", B2:B100)


5. Monthly Sales for Year 2024

Assuming "Date" is in Column E and "Sales Amount" is in Column B.

Use a Pivot Table with "Date" in Rows (grouped by month and year) and "Sales Amount" as Values (set to "Sum").

Formula to sum by month (assuming dates are in 2024):

=SUMIFS(B2:B100, E2:E100, ">=01/01/2024", E2:E100, "<=31/01/2024")


6. Top 5 Customers

Assuming "Customer Name" is in Column F and "Sales Amount" is in Column B.

Use a Pivot Table with "Customer Name" as Rows and "Sales Amount" as Values (set to "Sum"). Sort by "Sales Amount" in descending order and select the top 5.

Formula to find the highest sales for customers:

=LARGE(B2:B100, 1) for the highest, 2 for the second, and so on.


7. Total Sales by Day

Assuming "Date" is in Column E and "Sales Amount" in Column B.

Use a Pivot Table with "Date" in Rows and "Sales Amount" as Values (set to "Sum").

Formula for total sales by day:

=SUMIF(E2:E100, "Specific Date", B2:B100)

Replace "Specific Date" with the date for which you need total sales, or use cell reference if you have the date in another cell.
