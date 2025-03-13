# Home_Sales

## Home Sales Data Analysis with PySpark

This project analyzes home sales data using PySpark on **Google Colab**. The dataset is sourced from an **AWS S3 bucket**, and various queries are executed to extract insights related to home prices, bedrooms, bathrooms, square footage, and view ratings.

## Steps Performed:
1. **Set Up PySpark on Google Colab**  
   - Installed and configured Spark & Java.  
   - Initialized a SparkSession.

2. **Loaded Data from AWS S3**  
   - Read `home_sales_revised.csv` into a PySpark DataFrame.

3. **Created a Temporary SQL Table**  
   - Enabled SQL-based querying on the dataset.

4. **Executed Queries for Insights**  
   - Average home prices based on bedrooms, bathrooms, and square footage.  
   - Filtered data by conditions (e.g., homes with 3 beds, 3 baths, 2 floors).  
   - Analyzed home prices per view rating, filtering for values **≥ $350,000**.  

5. **Performance Optimization**  
   - Measured query runtime before and after caching the table.  
   - Saved data in **Parquet format**, partitioned by `date_built`.  
   - Compared query performance on CSV vs. Parquet formats.  

6. **Cleared Cached Data**  
   - Uncached the temporary table and verified its removal.

## Tools Used:
- **Google Colab** (for cloud-based execution)  
- **PySpark** (for big data processing)  
- **AWS S3** (for remote data storage)  

## Key Takeaways:
- Caching significantly **reduces query execution time**.  
- **Parquet format** improves efficiency over CSV.  
- Using **SQL on PySpark** simplifies complex data operations.  

