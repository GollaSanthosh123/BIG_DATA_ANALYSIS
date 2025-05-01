# Amazon Reviews Big Data Analysis using PySpark

This project showcases a basic big data analysis pipeline using **PySpark** on a sample Amazon product reviews dataset. It demonstrates how to load, clean, explore, and derive insights from large-scale text and numerical data efficiently using distributed computing.

## Project Overview

**Goal:** Analyze a large dataset using PySpark to extract meaningful insights such as:

- Most reviewed products
- Average star ratings by product
- Most active users (based on review count)

##  Dataset

A synthetic Amazon reviews dataset with **10,000 rows**, including:

- `review_id` (string)
- `product_title` (string)
- `customer_id` (int)
- `review_body` (string)
- `star_rating` (int)
- `review_date` (date)

##  Tools & Technologies

- Python 
- Apache Spark (PySpark)
- Google Colab / Jupyter Notebook (or any IDE with PySpark setup)
- Pandas / NumPy (used lightly for auxiliary tasks)

## Analysis Performed

### 1. Initialization
- Setup of `SparkSession`
- Imported necessary libraries

### 2. Data Loading & Exploration
- Loaded the dataset using `spark.read.csv(...)`
- Printed schema and initial sample
- Checked for missing values
- Descriptive statistics

### 3. Data Cleaning
- Dropped rows with null `review_body` or `star_rating`

### 4. Insight Extraction
- **Top Reviewed Products:** Identified products with the highest number of reviews
- **Average Ratings:** Calculated average star ratings per product
- **Most Active Users:** Found users with the most review submissions

##  Key Insights

-  **Most Reviewed Product:** *Wireless Earbuds* with 2029 reviews
-  **Highest Average Rating:** *Fitness Tracker* with an average of 3.05
-  **Most Active Users:** Several users submitted 3 or more reviews
2. Run the notebook or script:
   ```python
   spark-submit pyspark_amazon_analysis.py
   ```

3. View the output and modify for further analysis.
