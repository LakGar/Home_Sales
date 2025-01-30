# Home Sales Analysis

## Overview
This project uses **PySpark SQL** to analyze home sales data, perform queries, cache data, partition the dataset, and compare query performance.

## Files
- `Home_Sales.ipynb` - Jupyter Notebook with PySpark analysis
- `home_sales_revised.csv` - Dataset from AWS S3
- `README.md` - Project documentation

## Tasks
1. Load `home_sales_revised.csv` into a PySpark DataFrame.
2. Create a temporary table `home_sales`.
3. Answer the following queries:
   - Average price of four-bedroom houses sold per year.
   - Average price of homes built per year with three bedrooms and three bathrooms.
   - Average price of homes with three bedrooms, three bathrooms, two floors, and ≥2,000 sqft.
   - Average price per "view" rating for homes with an average price ≥ $350,000, including runtime.
4. Cache the `home_sales` table and validate caching.
5. Re-run the last query using the cached table and compare runtime.
6. Partition the dataset by `date_built` and store it in Parquet format.
7. Create a temporary table for the Parquet data.
8. Re-run the last query using the Parquet table and compare runtime.
9. Uncache the `home_sales` table and verify it.

## Technologies Used
- **Apache Spark** (PySpark SQL)
- **Jupyter Notebook**
- **Python**
- **AWS S3**
