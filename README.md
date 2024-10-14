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
1. The analysis results are summarized as follows:
2. The Coffee shop sales have been steadily increasing over the past months.
3. Mondays accounted for the highest total sales followed by Fridays and Thursdays.
4. The peak of sales activity during the day is at the 10th Hour.
5. There is high inflow of orders on Fridays compared to other weekdays.
6. Product of regular sizes are the most ordered from the findings.
7. The top selling product Category from this analysis is Coffee.

## Recommendations
Based on the analysis conducted, i recommend the following:
- There should be a Shift scheduling strategy of sales rep being targeted on fridays to ensure smooth and timely order processing and better customer experiences.
- To ensure a balanced customer to sales representative ratio, more sales reps should be placed between 8am and 9am daily on the selling floor.
- Promotions and Marketing campaigns should be targeted on Coffee Product category.



