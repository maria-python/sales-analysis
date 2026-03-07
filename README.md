# E Commerce Marketing Analysis
Author: Maria Ilnitsa

## Project Overview

This project analyzes marketing campaign performance and its relationship with customer behavior and sales outcomes in an e-commerce environment. Using datasets containing customer information, product catalog data, order transactions, and marketing campaigns, the analysis explores how marketing activities influence customer acquisition, purchasing patterns, and revenue generation.

The goal of the project is to transform raw business data into actionable insights that help the company optimize marketing spend, improve customer targeting, and increase overall revenue.


## Business Problem

An e-commerce company invests in multiple marketing campaigns but lacks clear visibility into how these campaigns influence sales performance and customer behavior.

The company wants to better understand:

- which marketing channels generate the most conversions

- how marketing campaigns influence customer acquisition

- which products and categories generate the highest revenue

- which customer segments drive the most sales

Management requires data-driven insights to optimize marketing strategy and allocate marketing budgets more effectively.


## Project Objectives

The main objectives of this analysis are:

- Identify sales performance trends

- Evaluate product and category revenue contribution

- Analyze customer purchasing behavior and segmentation

- Measure marketing campaign performance

- Calculate campaign conversion metrics

- Identify high-value products and customer segments

- Provide business recommendations for improving marketing effectiveness and revenue growth


## Analysis Hypotheses

## Dataset Overview

The project uses four datasets representing key areas of an e-commerce business:

### Customers

Information about customer demographics and signup behavior.

### Products

Product catalog data including product categories, pricing, and suppliers.

### Orders

Transaction-level data describing customer purchases.

### Campaigns

Marketing campaign data including campaign type, budget, clicks, and conversions.

The datasets contain **500 records each** and include information about:

- customer locations and segments  
- product categories and pricing  
- order quantities and payment methods  
- marketing campaign performance metrics  

Key variables include:

- Customer segment  
- Product category  
- Order quantity  
- Order revenue  
- Campaign type  
- Campaign budget  
- Clicks and conversions  

Key observations:

- Each dataset contains **500 rows**  
- Multiple relational tables simulate a real business database structure  
- Primary and foreign keys allow joins between tables  
- Data types were consistent and suitable for analysis  
- No missing values were detected during the preparation stage  


## Project Structure

```
sales_analysis
│
├── Data
│   └── campaings_data.csv
|   └── customers_data.csv
|   └── orders_data.csv
|   └── products_data.csv
│
├── Notebooks
│   └── analysis.ipynb
│
├── Visualization
│   └── .png
│   └── .png
|   └── .png
|   └── .png
|   └── .png
│
├── requirments.txt
|
├── README.md
|
└── DATASET_README.md

```


## Tools & Technologies

The analysis was conducted using the following tools:

- Python 3.11  
- Pandas – data manipulation and analysis  
- NumPy – numerical operations  
- Matplotlib – data visualization  
- Seaborn – statistical visualization  
- MySQL – relational database queries  
- Google Sheets – data exploration and dashboarding  
- VS Code & Jupyter Notebook
  

## Data Preparation

Several preprocessing steps were performed to prepare the datasets for analysis.

The `order_date` column was converted to datetime format to enable time-based analysis.

Additional time-based features were created:

- **Year** – order year  
- **Month** – order month  
- **Year_Month** – monthly period used for trend analysis  

Datasets were joined using relational keys:

- `customer_id` → linking customers and orders  
- `product_id` → linking products and orders  

This process enabled integrated analysis across customers, products, and transactions.

Additional calculated fields were created, including:

**Revenue = quantity × price**

This metric was used to analyze product performance and sales trends.


## Sales Analysis

## Customer Analysis

## Campaign Performance

## Conclusion

## Contact

Gmail: maria.ilnitska11@gmail.com

LinkedIn: www.linkedin.com/in/maria-ilnitska

Telegram: @mariailnitska
