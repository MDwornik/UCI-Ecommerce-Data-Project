# Ecommerce Sales and Customer Behavior Analysis

## Project Overview
This project analyzes ecommerce transaction data to understand customer behavior, product performance, and geographic trends. The analysis was conducted in Python for data preparation and Power BI for visualization.

The dataset contains over 500,000 transactions from a UK-based online retailer.

## Data
The original dataset is not included due to size constraints. 
It can be downloaded using the jupyter notebook or directly from the UCI Machine Learning Repository:

https://archive.ics.uci.edu/dataset/352/online+retail

## Objectives
- Analyze revenue trends over time  
- Identify high-value and at-risk customers  
- Evaluate product performance  
- Understand geographic distribution of revenue  
- Build an interactive dashboard for business insights  

## Tools and Technologies
- Python (Pandas, NumPy)  
- Power BI  
- Data cleaning and feature engineering  
- RFM segmentation  

## Data Preparation
The dataset required several preprocessing steps:

- Removed cancelled transactions
- Handled missing customer IDs
- Converted date columns to datetime format
- Standardized country values (e.g., "EIRE" to "Ireland")
- Created new features:
  - TotalPrice (Quantity × UnitPrice)
  - YearMonth, Hour, Day
  - DayOrder for proper weekday sorting

## Exploratory Analysis
Key analyses included:

- Revenue trends over time
- Revenue by day of week and hour
- Top customers by total spend
- Repeat vs one-time customers
- Product-level revenue and quantity
- Country-level revenue distribution

## Customer Segmentation (RFM)
Customers were segmented using:

- Recency: days since last purchase
- Frequency: number of orders
- Monetary: total spend

Segments include:
- Best Customers
- High Value At Risk
- Loyal but Inactive
- New Customers
- Lost Customers
- Average Customers

## Power BI Dashboard
The processed data was used to build a multi-page Power BI dashboard:

Executive Overview  
- KPIs (Revenue, Orders, Customers, AOV)
- Revenue trends over time
- Sales patterns by day and hour

Customer Insights
- RFM segmentation
- Customer value distribution
- Identification of high-value and at-risk customers

Product Performance
- Top products by revenue and quantity
- Revenue vs order volume analysis

Geographic Insights
- Revenue by country
- Regional performance comparison

## Key Insights
- Revenue is heavily concentrated in the United Kingdom
- Sales peak during midday hours and weekdays
- Revenue increases from September to November, indicating seasonality
- A small group of customers generates a large share of revenue
- Some high-volume products generate relatively low revenue, suggesting pricing opportunities

## How to Use
1. Run the Python notebook to reproduce the analysis
2. Load the generated CSV files into Power BI
3. Open the dashboard file to explore the results

## Future Improvements
- Cohort analysis for retention
- Customer lifetime value modeling
- Revenue forecasting
- Recommendation systems

## Author
Maciej Dwornik
