# Build-a-Retail-Data-Pipeline
In this project, I developed a data pipeline to analyze the impact of public holidays on Walmart's sales. By integrating and processing data from multiple sources, I created a comprehensive dataset to evaluate monthly sales trends, providing valuable insights into supply and demand dynamics around key holidays.

# Walmart Sales Analysis Project

## Overview
This project focuses on analyzing the supply and demand dynamics of Walmart around key public holidays. By integrating grocery sales data with complementary data, I aimed to understand how holidays such as the Super Bowl, Labour Day, Thanksgiving, and Christmas affect Walmart's sales performance.

## Data Sources
1. **grocery_sales** table from a PostgreSQL database:
   - `index`: Unique ID of the row
   - `Store_ID`: Store number
   - `Date`: The week of sales
   - `Weekly_Sales`: Sales for the given store

2. **extra_data.parquet** file containing complementary data:
   - `IsHoliday`: Indicates if the week contains a public holiday
   - `Temperature`: Temperature on the day of sale
   - `Fuel_Price`: Cost of fuel in the region
   - `CPI`: Consumer price index
   - `Unemployment`: Unemployment rate
   - `MarkDown1`, `MarkDown2`, `MarkDown3`, `MarkDown4`: Promotional markdowns
   - `Dept`: Department number in each store
   - `Size`: Size of the store
   - `Type`: Type of the store

## Project Steps
1. **Data Extraction**: Loaded the grocery_sales table from a PostgreSQL database and extra_data from a parquet file.
2. **Data Transformation**: Merged and cleaned the data to create a comprehensive dataset (`clean_data`).
3. **Analysis**: Conducted preliminary analysis to calculate monthly sales, resulting in the `agg_data` DataFrame.
4. **Output**: Saved the cleaned and aggregated data as CSV files for further analysis and reporting.

## Key Features
- **Integrated Data Pipeline**: Combines data from multiple sources to create a rich dataset for analysis.
- **Monthly Sales Analysis**: Evaluates the impact of public holidays on Walmart's sales, providing valuable business insights.
- **Efficient Data Handling**: Utilizes pandas for effective data manipulation and analysis.

## Installation and Usage
To replicate this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/walmart-sales-analysis.git
   cd walmart-sales-analysis

2. Install the required packages:
    ```bash
    pip install -r requirements.txt

3. Ensure you have access to the PostgreSQL database and the extra_data.parquet file. Update the database connection details in the script as needed.



4. Run the script to perform the analysis:
    ```bash
    python analyze_sales.py

## Results
The results of the analysis are saved in the following files:

clean_data.csv: The combined and cleaned dataset.
agg_data.csv: The aggregated monthly sales data.

## Conclusion
This project demonstrates my ability to build data pipelines, perform data integration, and conduct meaningful analysis to derive business insights. It highlights my skills in data manipulation, SQL, and Python, making me a strong candidate for data analysis and data engineering roles.

