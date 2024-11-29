# Coffee Shop Analysis

## Table of Contents
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Analysis Tools Used](#analysis-tools-used)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Findings](#findings)
- [Recommendations](#recommendations)
  
## Project Overview

This Data Analsis project aims to generate actionable insights from the retail sales data to enhance sales performance of the coffee shop.
By analyzing various aspect of the sales data, i seek to identify:
- How Sales vary by Day of the week and Hour of the day,
- The Total Sales Revenue for each Month
- How Sales vary across different Store locations,
- The Average Order and Sales per person,
- If there were pick times for Sales activities,
- The Variations in Size categories of products and
- The Best Selling Products Categories and Types.

![Screenshot 2024-10-14 193053](https://github.com/user-attachments/assets/48ecc8b4-3327-4741-97f7-ae39a884aa1e)



## Data Sources
Sales Data: The primary dataset used for this analysis is "Coffee Shop Sales" Excel file, containing detailed information of each sales made by the company. [Download here](https://mavenanalytics.io/data-Playground?order=date_added%2Cdesc&search=coff)

## Analysis Tools Used
- Microsoft Excel
- Power Query
- Power Pivot
- Power BI

## Data Cleaning and Preparation
In the initial Data Cleaning and Preparation Phase, i performed the following tasks:
1. Imported the data using power query
2. Used Power query to transform and add additional columns
3. Performed value replacement
4. Removed Duplicates
5. Handled Blanks and Trimmed Spaces

## Exploratory Data Analysis
EDA involves exploring the Sales Data to answer key questions, such as:
- How Sales vary by Day of the week and Hour of the day
- How Sales vary across different Store locations
- What are the peak selling period
- What are the best selling Products Categories and Types

![Screenshot 2024-10-14 195200](https://github.com/user-attachments/assets/31b28370-4538-4172-a132-377a135e9d81)

 
![Screenshot 2024-10-14 195046](https://github.com/user-attachments/assets/69bb0784-0689-40f2-8bba-20edc60aa55a)


![Screenshot 2024-10-14 195322](https://github.com/user-attachments/assets/cd843b3d-554b-4f53-891c-8a0a647c3bec)


![Screenshot 2024-10-14 195224](https://github.com/user-attachments/assets/cf196487-402c-44c6-a139-8cbad92eced3)


## Data Analysis
Power Pivot was used for creating some measures using DAX Funcions. Some of the measures used for these analysis include:
``` Sql
Total orders = COUNT('Data Cleaning & transformation'[transaction_id])
```
``` Sql
Total Sales = SUM('Data Cleaning & transformation'[Total Bills])
```
``` Sql
Avg Order per person = DIVIDE([Total Qty],[Total orders],0)
```
``` Sql
Avg Sale per Person = DIVIDE([Total Sales],[Total orders],0)
```

## Findings
 The analysis results are summarized as follows:
1. The Coffee shop sales have been steadily increasing over the past months.
2. Mondays accounted for the highest total sales followed by Fridays and Thursdays.
3. The peak of sales activity during the day is at the 10th Hour.
4. There is high inflow of orders on Fridays compared to other weekdays.
5. Product of regular sizes are the most ordered from the findings.
6. The top selling product Category from this analysis is Coffee.

## Recommendations
Based on the analysis conducted, i recommend the following:
- There should be a Shift scheduling strategy of sales rep being targeted on fridays to ensure smooth and timely order processing and better customer experiences.
- To ensure a balanced customer to sales representative ratio, more sales reps should be placed between 8am and 9am daily on the selling floor.
- Promotions and Marketing campaigns should be targeted on Coffee Product category.
- Regular and Large Sizes should be priotized during replenishments.



