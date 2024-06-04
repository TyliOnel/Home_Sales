# Home Sales Analysis with SparkSQL

## Overview
This project focuses on analyzing home sales data using SparkSQL, a powerful tool for big data processing. The goal is to extract key metrics and insights from the dataset, including average home prices based on various criteria such as the number of bedrooms and bathrooms, floor count, and view ratings. The analysis involves creating temporary tables, running complex SQL queries, and optimizing query performance through caching and data partitioning. By leveraging the capabilities of PySpark, this project aims to demonstrate efficient data processing and management techniques essential for handling large datasets in real-world scenarios.

## Instruction

### Data Processing and Analysis
1. **Import Libraries**
   - Import the necessary PySpark SQL functions.

2. **Read Data**
   - Read `home_sales_revised.csv` into a Spark DataFrame.

3. **Create Temporary Table**
   - Create a temporary table called `home_sales`.

4. **Run Queries**
   - Answer the following questions using SparkSQL:
     1. **Average Price for Four-Bedroom Houses:** Calculate the average price for a four-bedroom house sold for each year.
     2. **Average Price for Specific Three-Bedroom Houses:** Calculate the average price for three-bedroom, three-bathroom houses built each year.
     3. **Specific Three-Bedroom Houses with Criteria:** Calculate the average price for three-bedroom, three-bathroom houses with two floors and at least 2,000 square feet built each year.
     4. **Average Price per View Rating:** Calculate the average price of homes per "view" rating where the average price is at least $350,000. Measure the runtime.

### Optimization and Caching
1. **Cache Table**
   - Cache the `home_sales` temporary table and verify caching.
   - Run the last query using cached data and compare the runtime to the uncached version.

2. **Partition Data**
   - Partition the data by `date_built` and create a temporary table.
   - Run the last query on the partitioned data and compare the runtime to the uncached version.

3. **Uncache Table**
   - Uncache the `home_sales` temporary table and verify uncaching.

## Summary
In this project, I leveraged SparkSQL to perform comprehensive analyses on home sales data. By creating temporary tables, I was able to run complex queries to determine the average prices of homes based on various criteria, such as the number of bedrooms and bathrooms, floor count, and view ratings. I utilized caching to optimize query performance and partitioning to improve data management and query efficiency.

## Conclusion
The SparkSQL-based analysis of home sales data demonstrated the powerful capabilities of PySpark in handling large datasets and performing efficient data processing and querying. Through caching and partitioning, I significantly improved query performance, highlighting the importance of these techniques in big data processing. This project provided practical experience in using SparkSQL for real-world data analysis scenarios, showcasing its potential for scalable and efficient data management.
