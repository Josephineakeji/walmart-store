# Walmart Sales Data: End-to-End Analysis Pipeline

## Project Overview 

<img width="1598" height="753" alt="walmart_project-piplelines" src="https://github.com/user-attachments/assets/fd760fc3-07e6-44db-a902-88abaa078914" />
---

## Introduction:
This project focuses on a comprehensive analysis of **Walmart** sales data. The goal is to uncover hidden patterns in consumer behavior, branch performance, and product profitability. By leveraging a multi-tool approach, the project ensures data integrity through Python, deep exploration via SQL, and interactive storytelling through Power BI.

## Problem Statement:
- Identify branches experiencing a decline in revenue and understand the growth ratio between fiscal years.

- Determine peak business hours and the busy days to optimize staffing levels and inventory management.

- Distinguish between high-value and low-value items and understand which categories dominate market share.

- Pinpoint low-rated transactions and identify the highest-rated categories per branch to improve service delivery.

## Project Steps

### 1. Set Up the Environment
- **Tools Used**: Visual Studio Code (VS Code), Python, SQL (MySQL) and PowerBI
- **Goal**: Create a structured workspace within VS Code and organize project folders for smooth development and data handling.
  
### 2. Set Up Kaggle API
- **API Setup**: Obtain Kaggle API token from Kaggle by navigating to profile settings and downloading the JSON file.
- **Configure Kaggle**:
  - Place the downloaded `kaggle.json` file in local `.kaggle` folder.
  - Use the command `kaggle datasets download -d <dataset-path>` to pull datasets directly into project.

### 3. Download Walmart Sales Data
- **Data Source**: Use the Kaggle API to download the Walmart sales datasets from Kaggle.
- **Dataset Link**: [Walmart Sales Dataset](https://www.kaggle.com/datasets/najir0123/walmart-10k-sales-datasets)
- **Storage**: Save the data in the data/ folder for easy reference and access.
- 
### 4. Install Required Libraries and Load Data
- **Libraries**: Install necessary Python libraries using:
```
pip install pandas, numpy, sqlalchemy, mysql-connector-python
```
- **Loading Data**: Read the data into a Pandas DataFrame for initial analysis and transformations.
  
### 5. Explore the Data
- **Goal**: Conduct an initial data exploration to understand data distribution, check column names, types, and identify potential issues.
- **Analysis**: Use functions like `.info()`, `.describe()`, and `.head()` to get a quick overview of the data structure and statistics.
  
### 6. Data Cleaning
- **Remove Duplicates**: Identify and remove duplicate entries to avoid skewed results.
- **Handle Missing Values**: Drop rows or columns with missing values if they are insignificant; fill values where essential.
- **Fix Data Types**: Ensure all columns have consistent data types (e.g., dates as `datetime`, prices as   `float`).
- **Currency Formatting**: Use `.replace()` to handle and format currency values for analysis.
- **Validation**: Check for any remaining inconsistencies and verify the cleaned data.
  
### 7. Feature Engineering
- **Create New Columns**: Calculate the `Total Amount` for each transaction by multiplying `unit_price` by `quantity` and adding this as a new column.
- **Enhance Dataset**: Adding this calculated field will streamline further SQL analysis and aggregation tasks.
  
### 8. Load Data into MySQL 
- **Set Up Connections**: Connect to MySQL using `sqlalchemy` and load the cleaned data into the database.
- **Table Creation**: Set up tables in MySQL using Python SQLAlchemy to automate table creation and data insertion.
- **Verification**: Run initial SQL queries to confirm that the data has been loaded accurately.
  
### 9. SQL Analysis: Complex Queries and Business Problem Solving
- **Business Problem-Solving**: Write and execute complex SQL queries to answer critical business questions
  
- **Documentation**: Keep clear notes of each query's objective, approach, and results.

 ### 10. Visualization of Key Business Problems in PowerBI 

## Project Structure
```
|-- data/                     # Raw data and transformed data
|-- sql_queries/              # SQL scripts for analysis and queries
|-- notebooks/                # Jupyter notebooks for Python analysis
|-- README.md                 # Project documentation
|-- requirements.txt          # List of required Python libraries
|-- main.py                   # Main script for loading, cleaning, and processing data
```

## Results and Insights
This section will include your analysis findings:

- **Sales Insights**: Key categories, branches with highest sales, and preferred payment methods.
- **Profitability**: Insights into the most profitable product categories and locations.
- **Customer Behavior**: Trends in ratings, payment preferences, and peak shopping hours.

## Future Enhancements
Possible extensions to this project:

- Additional data sources to enhance analysis depth.
- Automation of the data pipeline for real-time data ingestion and analysis.

## License
This project is licensed under the MIT License.

## Acknowledgments
- **Data Source**: Kaggle’s Walmart Sales Dataset
- **Inspiration**: Walmart’s business case studies on sales and supply chain optimization.


