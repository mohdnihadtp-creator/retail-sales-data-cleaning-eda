# Retail Sales Data Cleaning & Exploratory Data Analysis (EDA)

Cleaning and exploring a raw retail sales dataset with Python to uncover what drives sales and profit.

## Project Overview
The raw dataset contained common data-quality problems such as extra whitespace, wrong data types, missing values and duplicate records. This project cleans the data and then analyzes sales and profit patterns across categories, customer segments, products and time.

## Dataset
File: `data/retail_sales_raw.csv`
Key columns: order date, ship date, customer name, city, segment, category, sub-category, product name, quantity, unit cost, unit selling price, discount, sales, profit, shipping cost, payment method.

## Data Cleaning Steps
- Removed leading/trailing whitespace from text columns
- Removed the `%` symbol from the discount column and converted it to numeric
- Standardized column names (lowercase, underscores)
- Converted sales and discount to numeric and order/ship dates to datetime
- Filled missing text values with "Unknown"
- Filled missing quantity and unit cost with the median, discount with 0
- Recalculated missing sales (quantity × unit selling price) and profit (sales − cost − shipping + adjustments)
- Filled missing dates with the most frequent date
- Removed duplicate records

## Analysis & Visualizations
- Correlation heatmap of numeric features
- Total sales by category
- Total sales by customer segment
- Total profit by category
- Monthly sales trend
- Top 10 products by sales
- Sales distribution (histogram)
- Profit distribution and outliers (box plot)
- Sales vs profit (scatter plot)

## Key Insights
- [Insight 1, e.g. "Category X generated the highest sales of ___"]
- [Insight 2, e.g. "Segment X contributed the most revenue"]
- [Insight 3, e.g. "Sales peaked in [month]"]
- [Insight 4, e.g. "Profit has outliers, suggesting unusual transactions"]

## Sample Visuals
![Correlation Heatmap](images/correlation_heatmap.png)
![Sales by Category](images/sales_by_category.png)
![Monthly Sales Trend](images/monthly_sales_trend.png)

## Tools Used
Python · Pandas · NumPy · Matplotlib · Seaborn · Google Colab / Jupyter Notebook

## How to Run
1. Clone this repository
2. Install dependencies: `pip install pandas numpy matplotlib seaborn`
3. Open `notebooks/retail_sales_eda.ipynb` in Jupyter or Google Colab
4. Run all cells

## Author
**Muhammed Nihad TP**
Aspiring Data Analyst / Data Scientist
LinkedIn:www.linkedin.com/in/muhammed-nihad-tpy
