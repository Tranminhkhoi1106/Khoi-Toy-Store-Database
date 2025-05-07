# Khoi-Toy-Store-Database
National Economic University FDA Project
Mavin ToyStore Dashboard
Dashboard link: https://app.powerbi.com/groups/me/reports/e322913e-8b07-4437-8085-26af56a870b7/329c6a152031d4eead26?experience=power-bi

Business Case: 
One beautiful morning, the CEO sends you— a Data Analyst— a message: "Some stores are not generating the expected profit. Find out why— using data!"
This project aims to analyze sales data to identify the reasons why certain stores are underperforming in terms of profitability. Additionally, it provides insights to help leadership and business teams determine which stores and products to focus on, optimizing sales and marketing strategies for the upcoming year.

Data:
- This project will utilize four available CSV files within the dataset:
- Products Table: Contains 35 products sold at Maven Toys (each record represents a product), with fields providing information on product categories, costs, and retail prices.
- Stores Table: Includes details about 50 Maven Toys store locations (each record represents a store), with fields covering store locations, business types, and opening dates.
- Sales Table: Holds data on the number of products sold across more than 800,000 transactions from January 2022 to September 2023 (each record represents the purchase of a specific product at a specific store on a specific date).
- Inventory Table: Contains inventory data for each product at various stores, including store codes, product codes, stock quantity, shortage levels, total inventory value, and out-of-stock status. This helps track goods and optimize restocking.

Steps:
#1: Data Cleaning:
- Download and Import: Retrieve CSV files and import them into Power BI Desktop.
- Data Transformation: Use Power Query to refine data before loading—check and adjust data types, rename columns within each table, remove unnecessary columns, eliminate duplicate records and blank rows, etc.
- Store Name Standardization: Shorten store names in the "stores" table to ensure consistency.
- Create new columns containing geographic information for cities and corresponding regions.
- Generate a universal date column with the earliest and latest dates from the actual dataset (Sales), adding new date-related columns such as year, month, etc., necessary for analysis.
- Include additional financial metrics such as Sales, Cost, and Profit to enhance analysis and provide deeper insights.

#2: Data Modeling:
- By working with a normalized database consisting of multiple interconnected tables, I harnessed Power BI's data modeling features to create logical and well-structured relationships between them. Utilizing the Relationship View, I carefully defined and managed these connections, ensuring a streamlined and integrated schema that promotes effortless data exploration and interaction.
- Establish relationships between data columns and the fact column using one-to-many relationships.
![image](https://github.com/user-attachments/assets/394e9a32-bc67-4fc6-b0bb-fba4521add5e)

#3: Data Analysis: Aggregate data and perform calculations to identify trends and relationships.
#4: Organization: Arrange raw fields, calculated columns, and key metrics into separate folders for easier navigation.
#5Report Structure: Divide the report into three pages: Summary, Store and Stock Analysis, and Product Analysis.
#6: Key Metrics: Include Total Sales, Profit, and Profit Margin across all pages, along with Total Units Sold for product performance evaluation. Additional metrics are also created to compare store performance.
#7: Data Visualization: Implement interactive visuals and parameterized metrics to enable stakeholders to explore data in-depth and interact dynamically with the multidimensional report.

Analysis:
Dashboard 1: Performance Analysis
![image](https://github.com/user-attachments/assets/0c70fc15-f5d0-4d43-88e0-8c533541c446)

- Key Metrics:
Total Sales: $14 Million
Total Profit: $4 Million
Profit Margin: 28%
Total Units Sold: 1.1 Million
- Profitability is strong at a 28% margin, suggesting efficient operations or premium pricing.
- Sales are highly concentrated in the Center region and downtown store locations—indicating a geographic and demographic skew. There may be an overdependence on a few strong markets.
- Toys dominate the product mix, both in share and growth, creating potential risk if demand shifts; diversification should be considered. However considered that the Data Date only take from 1/2022 ti 9/2023 so the comparison has lesser value.
- Although 2023 isn’t a full year yet, Art & Crafts sales have already surpassed 2022, which suggests a notable upward trend or seasonal acceleration. This likely indicates strong recent demand or successful promotions in that category. It's a special case where early-year performance is unusually strong, and if the trend holds, it could outperform expectations by year-end. This category deserves close monitoring and possibly increased investment to capitalize on the momentum.






