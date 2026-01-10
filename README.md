# Walmart Sales Data: End-to-End Analysis Pipeline

## Project Overview 

<img width="1598" height="753" alt="walmart_project-piplelines" src="https://github.com/user-attachments/assets/fd760fc3-07e6-44db-a902-88abaa078914" />
---

## Project Background:
In the competitive retail landscape, understanding the nuances of branch performance and consumer habits is vital for maintaining a market edge. This project establishes a robust, end-to-end data pipeline to analyze Walmart Sales Data.
By integrating Python for ETL (Extract, Transform, Load), MySQL for deep relational querying, and Power BI for visual storytelling, this pipeline transforms raw transactional records into actionable business intelligence. The primary objective is to solve operational bottlenecks regarding staffing, inventory allocation, and customer satisfaction.

Problem statement:
- Identify branches experiencing a decline in revenue and understand the growth ratio between fiscal years.

- Determine peak business hours and the busy days to optimize staffing levels and inventory management.

- Distinguish between high-value and low-value items and understand which categories dominate market share.

- Pinpoint low-rated transactions and identify the highest-rated categories per branch to improve service delivery.

## Data Structure & Initial Checks
The walmart database structure as seen below is a comprehensive table consisting of 
## 2. Data Structure Overview
 Below is the relational structure of the cleaned data:
<img width="325" height="382" alt="walmart ERD" src="https://github.com/user-attachments/assets/690b267c-d1bf-427a-ad69-66afa8c23209" />

Prior to the analysis, a series of rigorous preprocessing checks were performed on the raw dataset to address inconsistencies, handle missing values, and verify data types. The jupyter notebook with the data loading exploration and cleaning can be found [here](./notebooks/project.ipynb)



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


