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

---

## Key Insights

**1. Overall Discount Impact**
- **No Discount:** Highest total and average profits; steady growth over 2014-2017
- **Low (0-20%):** Moderately profitable; increases order volume while maintaining positive profits
- **Medium (20-35%):** Rarely profitable; generates losses. Not recommended.
- **High (35-50%):** Large negative profits; only for clearance or liquidation.
- **Mega (>50%):** Same effects as High discount

**Key Takeaway:** Discounts above 20% consistently reduce profitability

**2. Product Category Profitability**
- **Technology:** Best performer, tolerates low discounts.
- **Office Supplies:** Profitable only with no/low discounts; losses rise sharply beyond 20%
- **Mega Discounts:** Severely negative profits across all categories

**3. Customer Segment Profitability**
- **Low Discounts (<=20%):** Modestly profitable for all segments
- **Corporate:** Higher profit per order
- **Consumer:** Drives volume but must keep discounts <=20%

**4. Regional & State-Level Profitability**
- **Regions:** Profitable with no or low discounts; South and West most senstiive
- **Sates:** Top/Bottom states only profitable with <=20% discounts; mega discounts cause extreme losses

**5. Seasonal Patterns**
- **Q1 (Jan-Mar):** Lower profits; safest with no or low discounts
- **Q2-Q3 (Apr-Sept):** Low discounts maximize profits and volume
- **Q4 (Oct-Dec):** Non-discounted sales peak; high/mega discounts erode profits

**Overall Actionable Insights:**
To safeguard profits across products, customer segments, regions and seasons, keep discounts at or below 20%. For clearance or end-of life inventory, use larger discounts **only**

---

## Repository Structure
- `Profit_Optimization_DIscount_Strategy/`
  - `Data/`
    - `superstore.db`: relational database from the original dataset
    - `superstore_dataset.csv`: original dataset
  - `Visuals/`: images of graphs in the dashboard
    - `Dashboard_preview.png`: image of the final dashboard 
    - `Total_Profit_by_Category.png`
    - `Total_Profit_by_Segment.png`
    - `Total_Profit_by_State_and_Region.png`
    - `Total_Profit_by_Year_and_Month.png`
  - `notebooks/`
    - `Database_Deployer.ipynb`: code to create the tables and load data from original dataset into respective tables
    - `SQL_Query_Analysis.ipynb`: code done to perform calculation, aggregation, filtering and creating views
  - `Profit_Optimization_Dashboard.pbix`: final dashboard created of the results 
  - `requirements.txt`

---

## Dashboard Peview

![Dashboard Overview](https://github.com/KaiesoKB/Discount-Strategy-Analysis/blob/main/Profit_Optimization_DIscount_Strategy/Visuals/Dashboard_preview.png)

*Other sample visuals:*
- ![Profitability over Time](https://github.com/KaiesoKB/Discount-Strategy-Analysis/blob/main/Profit_Optimization_DIscount_Strategy/Visuals/Total_Profit_by_Year_and_Month.png)
- ![Profitability over Product Category](https://github.com/KaiesoKB/Discount-Strategy-Analysis/blob/main/Profit_Optimization_DIscount_Strategy/Visuals/Total_Profit_by_Category.png)
- ![Profitability over Customer Segment](https://github.com/KaiesoKB/Discount-Strategy-Analysis/blob/main/Profit_Optimization_DIscount_Strategy/Visuals/Total_Profit_by_Segment.png)
- ![Profitability over Customer State & Region](https://github.com/KaiesoKB/Discount-Strategy-Analysis/blob/main/Profit_Optimization_DIscount_Strategy/Visuals/Total_Profit_by_State_and_Region.png)

---
