# Home_sales
#Home_Sales Project

This repository encompasses a SparkSQL project designed to analyze home sales data. The project entails creating temporary views, partitioning data, caching and uncaching tables, and running SparkSQL queries to extract key metrics.

Project Structure

Home_Sales.ipynb: Jupyter Notebook containing the code for the SparkSQL project.
Data: Directory containing the dataset (home_sales_revised.csv) and formatted Parquet data.
README.md: This file provides information about the project.
Setup and Usage

Prerequisites
Ensure that you have a Python and PySpark environment set up.
Jupyter Notebook should be installed.
Project Setup
Clone the Repository:
bash
Copy code
git clone <repository-url>
cd Home_Sales
Download Data:
Download the Module 22 Challenge files and place them in the "Data" directory.
Notebook Execution:
Open and run the Home_Sales.ipynb notebook using Jupyter Notebook.
Project Overview

1. Creating Spark DataFrame
A Spark DataFrame is generated from the provided dataset (home_sales_revised.csv).

2. Creating Temporary Table
A temporary table named "home_sales" is formed using SparkSQL.

3. SparkSQL Queries
Various SparkSQL queries are formulated to address key questions about the home sales data:

Average price for a four-bedroom house sold for each year.
Average price of a home for each year it was built with three bedrooms and three bathrooms.
Average price of a home for each year with specific criteria (three bedrooms, three bathrooms, two floors, and >= 2,000 sq. ft.).
View rating for homes costing more than or equal to $350,000, with runtime measurement.
4. Caching and Uncaching
The temporary table "home_sales" is cached, and the cache status is checked. The same query is then run on both cached and uncached data to compare runtimes.

5. Parquet Data
The home sales dataset is partitioned by the "date_built" field, saved in Parquet format, and a temporary table is created for the Parquet data.

6. Uncaching and Verification
The temporary table "home_sales" is uncached, and the uncaching status is verified.

Evaluation

The project will be assessed based on the provided requirements. The grading criteria include the creation of Spark DataFrames, temporary tables, accurate SparkSQL queries, caching and uncaching, partitioning, and runtime comparisons.

License

This project is licensed under the MIT License.
