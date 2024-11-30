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

![Screenshot 2024-11-30 021304](https://github.com/user-attachments/assets/5cc48924-6284-40c6-bcac-90c5b4296e3a)

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
- How do Sales vary by Day of the week and Hour of the day?
- How do Sales vary across different Store locations?
- What are the peak time of selling activities?
- What are the best selling Products Categories and Types?
- Which Product Sizes is more profitable?

![Screenshot 2024-11-30 021828](https://github.com/user-attachments/assets/540bcd33-3fdc-48a5-ba33-ed9123b8668a)
![Screenshot 2024-11-30 021649](https://github.com/user-attachments/assets/2a9148a2-fbc7-4b9f-96e6-c45ab3ce9640)
![Screenshot 2024-11-30 021624](https://github.com/user-attachments/assets/28766736-4707-4d85-a77f-c66b38b29ee2)
![Screenshot 2024-11-30 021602](https://github.com/user-attachments/assets/50196260-2cf2-4649-a542-6a8227095862)
![Screenshot 2024-11-30 021440](https://github.com/user-attachments/assets/21b02add-8190-405f-bc34-906ca29833c2)
![Screenshot 2024-11-30 021927](https://github.com/user-attachments/assets/ed14e657-2407-4793-9bac-a507f5f415eb)


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



