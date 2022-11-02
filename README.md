# Adebowale-Sagbele-Portfolio
Analytics Portfolio

# [Project 1: Customer Profiling Using Cluster Analysis](https://github.com/vsthepen/Telecomms-Dashboard)

This analytics project was imperative for stakeholders of ABC Telecomms to support their revenue drive and marketing effort. They wanted to have a better understanding of their customers, especially with regards to how they use their Internet Data Plans.
The company provided 6 months of customer data for profiling before further analysis.

First step:  I imported and cleaned the data contained in an excel workbook via power query editor in power bi. Unwanted columns, empty cells and redundant data were eliminated. Also, data types for each column were validated to maintain accuracy.

Second step: Normalized the data and established relationships between the fact and dimension tables using the customer number as the unique key.

Third step: Loyalty scores were assigned to each customer based on Data Subscribed and Bonus usage. Using on the customers final score, customers were classified into the following:
- Tier 1 Priority Service – Above 85% 
- Tier 2 Priority Service – Between 75% and 85%
- Tier 3 Priority Service + Incentives – Above 60% and less than 75%
- Tier 4 Priority Marketing + Incentives – Less than or equal to 60% 

In addition, key measures including Total number of customers, Total Assigned score, % Assigned score, Customer Group were created using Dax formulas.

Fourth step: A dynamic dashboard was created showing the 4 customer tiers with the aid of a bar chart, which is a great choice for visualizing data with less than 5 categories. A donut chart was also utilized to show the percentage of customers by city.

## ABC Telecomms Dashboard Showing Customer Tiers
![ABC DASHBOARD-1](https://user-images.githubusercontent.com/115559534/199286385-9512d81d-fbbd-4e5c-962e-951b3c7d4957.png)

# Challenges Encountered
1. Assigning customer group/tier to each customer based on their final score.
- SOLUTION: I joined the power Bi community online where I was guided on how to use the SWITCH function.

2. Some customers subscribed for data multiple times in a month, therefore the data subscribed & bonus used for that month had to be summed into one row and grouped into one Customer Number.
- SOLUTION: I did some research online and eventually spoke to a colleague who told me about the “group by” function in power query.

# [Project 2: Sales Trend, Product Sales & Sales Performance Analysis](https://github.com/vsthepen/Sales-Trend-Analysis)

The executive management of Mark Up Foods and Beverages requested for a sales trend and product sales analysis report to enable them gain insights into the top performing and underperforming products, also to evaluate sales team performance between 2019 and 2021. The data was collected in 3 separate excel workbooks for each year. Each workbook contained similar columns such as salesperson, orders, order Date, product group, quantity, unit price, etc. The sales budget data for each year was equally provided. The data was then extracted and transformed using the power query editor.

First Step: I ensured that totals, subtotals, empty rows, and columns were removed from the tables. I also checked that all columns had a first row of descriptive heading. Furthermore, data types for each column were validated to ensure correctness.

Second Step: After the data cleaning process, the three separate tables for each year were appended into one since they had the same exact headers and contained similar information. Thereafter, tables not needed in the model were disabled leaving only one big fact table.

Third step: The data in the fact table was normalized. This resulted in the creation of 2 dimension tables which includes the Product and Salesperson table. I ensured that the dimension tables only contained unique values i.e., duplicates were removed.

Fourth step: The fact and dimension tables were loaded onto the power bi report page. Relationships were created between the tables with the help of unique keys i.e., Salesperson key and Product ID.

Measures such as Total Budgeted Sales, Total Actual Sales, Total Quantity Sold, Rank for Salesperson, % Budgeted sales vs Actual were calculated by using DAX.

Fifth Step:  A sales trend dashboard was built showing the total sales by product group, quarterly & yearly sales trend. This was visualized with the aid of a clustered bar chart and an area chart respectively.
## Sales Trend Dashboard
![MARK UP FOODS AND BEVERAGE-2](https://user-images.githubusercontent.com/115559534/199511693-d1d90215-8f3d-499f-a4ce-02629ca5b818.png)

A Sales Team dashboard was additionally created to display the Quantity sold by Salesperson, Actual vs Budgeted sales for each person and the Top 3 Salespersons by Sales Amount. A bar chart, line chart and a multi row card were used respectively.
## Sales Team Performance Dashboard
![MARK UP FOODS AND BEVERAGE-3](https://user-images.githubusercontent.com/115559534/199512100-9892749d-2297-41f6-954b-df6cf4f4bc24.png)

I tried my hands on the customized tool tips options within Power Bi to give my dashboard a more professional face lift especially during presentations.
## Customized tooltip
![image](https://user-images.githubusercontent.com/115559534/199511276-fc20f100-d18f-43e8-9374-4924850aa93f.png)

# Challenges Encountered
- Incorporating images for salespersons into the report. I found the solution after going through a few YouTube videos.
- Using conditional formatting on the line chart to show GREEN when Actual Sales > Budgeted Sales, 
RED when Budgeted Sales > Actual Sales. I also found the solution to this after 30 to 45 minutes of YouTube research.

In conclusion, I enjoyed every bit of working on this project, can you tell?.






