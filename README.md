![image](https://github.com/user-attachments/assets/3759adad-2e78-4eec-b0de-90157cc07e18)# Khoi-Toy-Store-Database
National Economic University FDA Project
Mavin ToyStore Dashboard
Dashboard link: https://app.powerbi.com/groups/me/reports/e322913e-8b07-4437-8085-26af56a870b7/329c6a152031d4eead26?experience=power-bi

I. Business Case: 
One beautiful morning, the CEO sends you— a Data Analyst— a message: "Some stores are not generating the expected profit. Find out why— using data!"
This project aims to analyze sales data to identify the reasons why certain stores are underperforming in terms of profitability. Additionally, it provides insights to help leadership and business teams determine which stores and products to focus on, optimizing sales and marketing strategies for the upcoming year.

II. Data:
- This project will utilize four available CSV files within the dataset:
- Products Table: Contains 35 products sold at Maven Toys (each record represents a product), with fields providing information on product categories, costs, and retail prices.
- Stores Table: Includes details about 50 Maven Toys store locations (each record represents a store), with fields covering store locations, business types, and opening dates.
- Sales Table: Holds data on the number of products sold across more than 800,000 transactions from January 2022 to September 2023 (each record represents the purchase of a specific product at a specific store on a specific date).
- Inventory Table: Contains inventory data for each product at various stores, including store codes, product codes, stock quantity, shortage levels, total inventory value, and out-of-stock status. This helps track goods and optimize restocking.

III. Steps:
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

Performance Dashboard: ![image](https://github.com/user-attachments/assets/9682abe3-df93-4bfe-be0c-8e7a8e4d779e)
Store Analysis Dasboard: ![image](https://github.com/user-attachments/assets/c67a77ed-40e1-4c49-b2fd-0bad78eafcb1)
Inventory Dashboard: ![image](https://github.com/user-attachments/assets/23802d1a-f2e7-4497-b12c-18eb81d3cd08)



IV. Analysis:

Dashboard 1: Performance Analysis

- Key Metrics:
Total Sales: $14 Million
Total Profit: $4 Million
Profit Margin: 28%
Total Units Sold: 1.1 Million
- Profitability is strong at a 28% margin, suggesting efficient operations or premium pricing.
- Sales are highly concentrated in the Center region and downtown store locations—indicating a geographic and demographic skew. There may be an overdependence on a few strong markets.
- Toys dominate the product mix, both in share and growth, creating potential risk if demand shifts; diversification should be considered. However considered that the Data Date only take from 1/2022 ti 9/2023 so the comparison has lesser value.
- Although 2023 isn’t a full year yet, Art & Crafts sales have already surpassed 2022, which suggests a notable upward trend or seasonal acceleration. This likely indicates strong recent demand or successful promotions in that category. It's a special case where early-year performance is unusually strong, and if the trend holds, it could outperform expectations by year-end. This category deserves close monitoring and possibly increased investment to capitalize on the momentum.

Dashboard 2: Store Analysis

1. For store locations, analyze sales and compare them with inventory data. Are there any stock shortages, as sales cannot occur without available products?

This report aims to assess the financial consequences of product unavailability, with a particular focus on revenue loss due to stockouts at various locations. Understanding this impact is crucial for optimizing inventory management and maximizing sales potential. To achieve this goal, the following key metrics will be analyzed for each location:

- Potential Revenue:
This metric represents the maximum theoretical revenue that could be achieved at each location, assuming all products are always available to meet customer demand. It serves as a benchmark for comparison with actual performance, highlighting the full market potential of each site.

- Actual Revenue:
This is the total revenue generated at each location during the reporting period, taking into account the actual availability of products. It reflects the tangible sales achieved despite any stockout situations.

- Lost Revenue:
This critical metric quantifies the revenue shortfall that directly results from periods when specific products were unavailable for purchase. It isolates the financial impact of stockouts by estimating the sales that could have been made from these out-of-stock items if they had been in stock. It represents the direct loss of potential income.

- Percentage of Lost Revenue:
To provide a clear and comparable measure of the impact of stockouts, this metric calculates the proportion of potential revenue that was not realized due to product unavailability. Expressed as a percentage, it offers a standardized way to assess the severity of stockout issues across different locations, regardless of their total sales volume. This allows stakeholders to quickly identify areas where stockout management requires the most attention.

![image](https://github.com/user-attachments/assets/b99d0735-78bd-458c-95c7-38aa5db283bd)

From the above data, Residential and Downtown are the two locations with the highest percentage of lost revenue—4.96% and 2.63%, respectively. This strongly suggests that frequent stockouts in these areas are negatively impacting financial performance. Notably, Downtown has a relatively large number of stores (29), yet still experiences significant revenue loss due to stock shortages. Even the top-performing store in the Residential area suffers from revenue loss caused by product unavailability.

➡ Conclusion: The lower profit margins observed in Residential and Downtown are likely driven by recurring stockouts. These shortages not only limit actual sales but also contribute to missed revenue opportunities and risk diminishing customer satisfaction and loyalty.

Interestingly, 3 out of the top 5 stores by total sales and profit are located in Downtown, and these stores did not experience stock shortages. This implies that Downtown has strong revenue-generating potential when inventory is well managed.

💡 Insight & Recommendation:

- Residential emerges as a key area of concern. Despite having high demand, it suffers from the highest percentage of lost revenue. This indicates untapped potential that could be unlocked with better inventory control and supply chain responsiveness.

- A targeted strategy to improve stock availability in Residential stores could significantly increase revenue and overall profit margins.

- For Downtown, focus on replicating the operational efficiency of its best-performing stores across all outlets to minimize lost revenue and maximize return on investment.

- A deep-dive analysis into the inventory management systems and forecasting methods in these two regions is recommended to identify root causes and develop tailored solutions.

2. Store_Location can affect customer traffic. Are there any locations that are less favorable compared to others?

![image](https://github.com/user-attachments/assets/6a93420e-3fb7-4340-b5bd-2238b5c58f56)

 Nearly 60% of all Maven Toys stores are located in Downtown. On average, Airport stores generate the highest daily revenue per store at $708—over 30% more than stores in other areas. While Airport shows strong potential for expansion, it may also require significant investment, which warrants further evaluation.
Key Insights:
- Downtown dominates in store count with 29 stores but contributes only 11.47% of total revenue and has the lowest profit margin (27%). High operating costs or lower pricing may be factors.
- Airport leads in profitability, generating 56.9% of total revenue with the highest profit margin (29%), despite fewer stores.
- Commercial and Residential show stable performance with 28% margins and contribute 22.7% and 8.93% of revenue respectively.
Opportunities:
- Airport should be explored for expansion, though investment needs must be considered.
- Downtown needs cost or pricing strategy optimization to boost margins.
- Commercial & Residential can be further optimized through customer behavior insights.

➡ Before deciding on a target area for expansion, a key question remains: Is there a correlation between the number of stores in a city and the total revenue generated?
![image](https://github.com/user-attachments/assets/de5661d3-4605-42f7-9129-ac14459cc54f)

The answer is yes. There is a strong positive correlation between the number of stores in a city and the revenue generated in that city. This means that as the number of stores in a city increases, the amount of revenue generated also rises. However, it is important to note that there may be a hidden variable influencing the sales volume at stores in each city.

Dashboard 3: Inventory Analysis
3. Which products are actually generating profit? Is this consistent across all store locations?
![image](https://github.com/user-attachments/assets/69565e2a-db76-4953-aee6-5eaea0b065bf)


Across store regions, Toys (Lego Bricks and Action Figure) and Electronics (Colorbuds) continue to be the highest-profit categories.
Electronics generates the most profit at Airport ($108,197) and Commercial ($287,574) store locations.
Meanwhile, Toys is the top profit-generating category at Downtown ($630,029) and Residential ($136,214).

4. Are there seasonal factors affecting product sales? When is the peak selling period?
![image](https://github.com/user-attachments/assets/a0604088-fcc4-4d18-b3c4-f715f4f90e18)

- The data shows that sales steadily increased from January ($542,554) to April 2022 ($681,072). Afterward, the sales trend declined until August ($489,422). Since this period coincides with summer, people tend to engage more in outdoor activities, which could explain the drop in sales.

- Following August, monthly sales consistently increased from $585,844 in September to $661,304 in November. These three months of growth peaked with a sharp spike to $877,203 in December, the highest recorded monthly sales. This year-end surge was likely driven by high demand for Christmas purchases.

- In 2023, monthly sales declined for two months, reaching $722,632 in February, but then rebounded significantly in March to $883,515. Over the next six months, sales trends followed a similar pattern to 2022, remaining relatively stable from April to June, before dropping again between July and September.

- Notably, as of September 2023 ($6.96 million), cumulative sales had already surpassed the cumulative sales at the same time in September 2022 ($5.32 million). Given that total sales for 2022 reached $7.48 million, and 2023 sales data continues to follow a similar trend, Maven Toys can reasonably expect to exceed that figure by the end of the year.

![image](https://github.com/user-attachments/assets/5bb04ac8-4346-4ebf-86ca-ca1d5a74b9a8)

Although Electronics is the second most profitable category, its monthly sales have steadily declined, dropping from $143,088 in January 2021 to $72,547 in September 2022. This downward trend contrasts significantly with the Toys category, which has remained relatively stable. Additionally, Toys experienced growth in both summer 2022 and winter 2024, likely due to summer vacations and year-end holiday seasons. While demand for Electronics has declined, demand for Toys has remained unchanged.

So, when one of the highest-revenue product categories has been experiencing declining sales for the past 20 months, the question arises: How is the company still on track to surpass the total sales of 2022?
![image](https://github.com/user-attachments/assets/c99235cc-a70f-45b6-9211-67cf267fb3a6)
![image](https://github.com/user-attachments/assets/d528f9c9-bae8-4042-91be-7fcf81bba113)

→ With one of the primary profit-generating product categories experiencing declining sales for the past twenty months, it raises the question of how the company is still on track to surpass total sales for 2022. The answer lies in the significant growth of the Arts and Crafts category.

Monthly sales have shown an upward trend, increasing from $35,097 in January 2022 to $187,299 in September 2023, with a peak of $230,299 in April 2023. Leveraging this rising demand could further drive sales growth for Maven Toys.






