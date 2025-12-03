📈 Stock Market Data Validation & Analysis (End-to-End Data Pipeline Project)

📌 Project Overview

    This project analyzes daily stock market trends using live financial data, focusing on data extraction, cleaning, validation,SQL storage, and visualization.

    It demonstrates how a data analyst ensures data quality, pipeline accuracy, and actionable insights.

This project showcases:

    End-to-end ETL pipeline (Extract → Transform → Load)
    Automated data validation using SQL & Python
    Stock trend data analysis
    SQL-based data storage
    Power BI visualization
    Real-world data quality (DQ) checks

🧩 Project Components

1. Data Extraction (Python + API)

    Source: Yahoo Finance (yfinance)
    Fetches multiple stock symbols
    Hourly/daily prices stored in data_raw/

2. Data Cleaning & Transformation

    Standardize column names
    Convert timestamps
    Calculate % change & daily returns
    Store cleaned files in data_clean/

3. Data Validation (SQL + Python)

    Includes:
        Null checks
        Duplicate detection
        Negative/zero price checks
        Outlier detection
        Price consistency validation
        Row count comparison
        Validation logs

4. SQL Database Storage

    Cleaned data is inserted into table:
        daily_stock_data(symbol, datetime, open_price, high_price, low_price, close_price, volume, change_pct)

5. Automated Pipeline

    Using:
        <!-- Windows Task Scheduler
        Linux Cron Job -->

Automation steps:
    
    Fetch data,
    Clean data,
    Validate data,
    Insert to SQL,
    Log results.

6. Data Analysis & Insights

    Visualized in Power BI:
        Closing price trends,
        Top gainers/losers,
        Volume trends,
        Daily percentage change,
        Moving averages.
