# 💰Profit Optimization Through Discount Stategy Analysis
In order to assists retailers in creating more intelligent, data-driven promotional strategies, this project examines the connection between discount levels and profitability. To determine the most lucrative discount ranges across products, customer segments, regions, states, and time periods; historical retail sales data was ingested, examined, and visualized using Python SQLite, and power BI. 

---

## Objective/Purpose
This project's goal is to assess how various discount levels affect profitability for various producst, clientele groups, geographical areas, and time periods. The study provides actionable insights to support more intelligent retail promotion strategies by analyzing historical sales data to determine discount ranges that maximize profit.

---

## Data Source & Tools Used
- **Data Source:** [Superstore Dataset (Kaggle)](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)

- **Tools & Libraries:**
  - **Python:** pandas, numpy, Jupyter Notebook
  - **SQLite3:** for database creating and SQL queries
  - **Power BI Desktop:** for dashboard design and visualization
  - *(Optional)* matplotlib, seaborn for data exploration

---

## Project Workflow

1. **Data Preparation & Database Creation**
   - Loaded the original CSV data into Python.
   - Transformed the data.
   - Built and populated an SQLite database with four related tables: `customers`, `products`, `orders`, `order_details`
2. **Analysis & SQL Queries**
   - Queries the database using SQLite and pandas to calculate key metrics:
     - Number of Orders
     - Total Sales
     - Total Profit
     - Average Profit
     - Profit Margin
   - Grouped and aggregated results by discount range, product cateogory, customer segment, region, state, and time
3. **Visualization & Dashboard**
   - Imported the database into Power BI Desktop
   - Created and interactive dashboard with filters for discount range, time and region
   - Key charts hightight profitability trends

