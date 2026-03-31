Nashville Housing Data Cleaning and Preparation Using SQL

Summary:
This project focuses on cleaning and preparing a real-world housing dataset using SQL. The goal was to improve data quality, consistency, and usability for further analysis. Key tasks included standardizing date formats, handling missing values, splitting complex columns, removing duplicates, and transforming categorical data. The cleaned dataset is structured to support more accurate reporting, analysis, and visualization.

Business Problem:
Raw datasets often contain inconsistencies such as missing values, duplicate records, and poorly formatted fields. In this case, the Nashville Housing dataset had issues, including inconsistent date formats, missing property addresses, combined address fields, duplicate records, and non-standard categorical values. These issues can lead to inaccurate analysis and unreliable insights. The objective was to clean and standardize the dataset to make it analysis-ready. 

Methodology:
1. Queried the Nashville Housing dataset to explore its structure and identify issues such as missing values, inconsistent formats, and duplicates.
2. Standardized the SaleDate format by converting it into a consistent date type and creating a new column for easier analysis.
3. Filled missing property address values by using self-joins on ParcelID to ensure more complete records.
4. Transformed the dataset by splitting PropertyAddress and OwnerAddress into separate columns for address, city, and state.
5. Cleaned categorical data by converting values such as Y/N into standardized Yes/No labels.
6. Identified and removed duplicate records using a CTE with ROW_NUMBER() based on key fields.
7. Optimized the dataset by removing unnecessary columns to improve structure and query efficiency.

Skills:
1. SQL: CTEs, Joins, CASE statements, aggregate functions, window functions (ROW_NUMBER), data cleaning, and transformation
2. Data Cleaning Techniques: Handling NULL values (ISNULL), string manipulation (SUBSTRING, PARSENAME), data standardization, and duplicate removal
3. Data Preparation: Column splitting, data normalization, schema modification (ALTER TABLE), data quality improvement
