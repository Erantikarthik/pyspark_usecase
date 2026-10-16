# Distributed Data Processing with PySpark

## Project Overview

This project demonstrates how to process and analyze e-commerce order data using PySpark in Databricks Free Edition. It covers data cleaning, duplicate removal, data transformation, and sales analysis.

## Technologies Used

- Python
- Apache Spark (PySpark)
- Databricks Free Edition
- Delta Lake
- Git and GitHub

## Project Workflow

1. Created a sample e-commerce orders dataset.
2. Removed records with missing customer names or product values.
3. Filtered out invalid prices and quantities.
4. Removed duplicate order IDs.
5. Calculated total sales for each order.
6. Aggregated revenue and order counts by product.
7. Saved processed data as a Delta table in Databricks.
8. Exported the processed results to CSV.

## Data Quality Checks

- Removed records with missing customer names or product values.
- Excluded records with non-positive prices or quantities.
- Removed duplicate order IDs.
- Retained 7 valid orders from the original 11 records.

## Key Results

| Metric | Result |
|---|---:|
| Original records | 11 |
| Cleaned orders | 7 |
| Total revenue | ₹345,000 |
| Average order value | ₹49,285.71 |
| Highest-revenue product | Laptop |
| Laptop revenue | ₹220,000 |

## Project Files

- `Distributed_Data_Processing_PySpark.ipynb` — notebook containing the PySpark processing workflow.
- `processed_sales.csv` — cleaned and transformed order data.
- `README.md` — project documentation.
- `.gitignore` — excludes specified temporary files and local configuration.

## Limitations

This project uses a small sample dataset for learning and demonstration. Some RDD operations were not executed because SparkContext access is restricted in Databricks Serverless.

## Future Improvements

- Process a larger real-world dataset.
- Add automated data validation checks.
- Implement incremental data processing.
- Schedule pipeline execution.
- Build a Power BI dashboard for sales analysis.

## Author

**Eranti Karthik**

GitHub: https://github.com/Erantikarthik

## Project Repository

https://github.com/Erantikarthik/pyspark_usecase