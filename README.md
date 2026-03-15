# E Commerce Marketing Analysis
Author: Maria Ilnitsa

## Project Overview

This project analyzes sales performance, customer purchasing behavior, and marketing campaign effectiveness in an e-commerce environment. The analysis uses multiple relational datasets containing information about customers, products, orders, and marketing campaigns.

The goal of the project is to transform raw transactional and marketing data into actionable business insights that help improve revenue generation, customer retention, and marketing efficiency.

By combining sales data with customer segmentation and campaign performance metrics, the analysis identifies key drivers of revenue and opportunities for improving marketing strategy.


## Business Problem

An e-commerce company collects large amounts of data related to customer purchases, product sales, and marketing campaigns. However, management lacks clear visibility into:

- which products and categories generate the most revenue

- how customer behavior impacts sales performance

- which marketing channels are most effective at converting users into customers

- how customer segments contribute to overall revenue

Without structured analysis, it is difficult to make data-driven decisions about marketing investments, product strategy, and customer retention.


## Project Objectives

The main objectives of this analysis are to:

- analyze overall sales performance and revenue distribution

- identify top-performing products and product categories

- examine customer purchasing behavior and repeat purchase patterns

- evaluate marketing campaign performance using key marketing metrics

- measure conversion efficiency across marketing channels

- identify opportunities to improve customer retention and marketing effectiveness


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
  

## Data Preparation & KPI Metrics

Several preprocessing and metric calculation steps were performed to ensure the datasets were clean, consistent, and ready for analysis.

### 1. Quick Data Overview
- Applied `.head()` and inspected columns for all datasets: `orders`, `customers`, `products`, `campaigns`.  
- Verified column names, data types, and initial sample values.  

### 2. Quick Data Checks
- Performed preliminary validation for each dataset:  
  - **Orders**: checked `quantity`, `total_price`, `order_status`  
  - **Customers**: verified `customer_segment`, `signup_date`, `country`/`city`  
  - **Products**: reviewed `price`, `cost`, `category`  
  - **Campaigns**: inspected `start_date`, `end_date`, `budget`, `clicks`, `conversions`  

### 3. Date / Time Preprocessing
- Converted all date columns from strings to `datetime` objects (`pd.to_datetime`) for accurate time-based analysis.  
- Applied to:  
  - **Orders**: `order_date`  
  - **Customers**: `signup_date`  
  - **Campaigns**: `start_date` and `end_date`  

### 4. Feature Engineering
- Created new columns to support trend analysis and aggregation:  
  - **Orders**: `Year`, `Month`, `Year_Month` based on `order_date`  
  - **Customers**: `Year`, `Month` based on `signup_date`  
  - **Campaigns**: `Start_Year`, `Start_Month`, `End_Year`, `End_Month` based on campaign dates  

### 5. KPI / Metrics Calculation
To measure marketing performance, several key metrics were calculated for each campaign:

- **Conversion Rate (CR)** = `conversions / clicks`  
- **Cost per Click (CPC)** = `budget / clicks`  
- **Cost per Acquisition (CPA)** = `budget / conversions`  

Handling divide-by-zero:  
- Replaced infinite values from 0 conversions or clicks with `pd.NA` to avoid errors in analysis.

Example of calculated metrics for campaigns:

| campaign_id | campaign_name | CR   | CPC    | CPA    |
|------------:|---------------|------|--------|--------|
| 1           | Campaign_1    | 0.441 | 2.27   | 2.27   |
| 2           | Campaign_2    | 0.006 | 8.64   | 8.63   |
| 3           | Campaign_3    | 0.119 | 2.36   | 2.36   |

These metrics provide the foundation for evaluating campaign effectiveness and optimizing marketing spend.

### 6. Data Preparation Complete
- All datasets are now ready for:  
  - relational joins between orders, customers, products, and campaigns  
  - KPI and revenue analysis  
  - customer segmentation and campaign performance evaluation  

This structured preparation ensures a clean foundation for subsequent analysis of marketing, sales, and customer behavior. 


## Sales Analysis

## Customer Analysis

## Campaign Performance

## Conclusion

## Contact

Gmail: maria.ilnitska11@gmail.com

LinkedIn: www.linkedin.com/in/maria-ilnitska

Telegram: @mariailnitska
