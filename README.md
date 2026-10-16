# Distributed Data Processing with PySpark

## Project Overview
This project demonstrates distributed data processing using PySpark in Databricks. It uses sample e-commerce order data to explore, clean, transform, and analyze sales information.

## Technologies Used
- Databricks Free Edition
- Apache Spark
- PySpark
- Python
- Spark DataFrames
- Git and GitHub

## Project Workflow
1. Initialize the Spark session.
2. Create a sample e-commerce dataset.
3. Explore records, schema, data types, and summary statistics.
4. Identify missing values.
5. Remove rows with missing customer names or products.
6. Filter out invalid prices and quantities.
7. Remove duplicate order IDs.
8. Calculate total order amounts.
9. Analyze revenue by product and customer.
10. Apply transformations and filters.
11. Save processed sales data as a Delta table, where supported.

## Data Cleaning
The sample dataset contains 11 original records. The cleaning process removes records with missing required values, invalid prices or quantities, and duplicate order IDs.

The resulting dataset contains 7 records.

## Results
- Cleaned orders: 7
- Total revenue: 345,000
- Average order value: 49,285.71

### Product-wise Revenue

| Product | Revenue | Orders |
|---|---:|---:|
| Laptop | 220,000 | 3 |
| Mobile | 80,000 | 2 |
| Tablet | 45,000 | 2 |

## Learning Outcomes
- Working with Spark DataFrames
- Cleaning and validating data
- Performing distributed transformations and aggregations
- Calculating sales metrics
- Using Databricks Serverless compute

## Limitations
Traditional RDD operations requiring direct SparkContext access were not executed because Databricks Serverless does not support that access.

## Future Improvements
- Process larger datasets.
- Add automated data quality checks.
- Build a scheduled data pipeline.
- Extend the project with Bronze, Silver, and Gold layers.
- Add further performance and scalability experiments.