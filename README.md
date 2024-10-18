## Avocado Bag Size Sales Percentage Analysis

## Project Overview
This project analyses the monthly sales percentages of different avocado bag sizes (small, large, and x-large) across various regions using BigQuery. The goal is to understand how each bag size performs in terms of sales volume, helping to draw insights on trends over time and across regions.

## Data Source
The dataset used for this analysis is sourced from Kaggle: Avocado Prices Dataset, and is licensed under the Open Data Commons Open Database License (ODbL) v1.0. You can download the dataset from Kaggle directly.

## Data License Information:
The dataset is licensed under the Open Data Commons Open Database License (ODbL) v1.0. This means:

You can share, modify, and use the dataset as long as you attribute the source.
Any modifications or derivative datasets must be shared under the same ODbL license.
Always ensure the data remains open and accessible.
More information on the license can be found here.

Note: I have not uploaded the dataset itself to this repository due to the licensing terms. Please download the dataset from Kaggle if you wish to replicate this analysis.

## Objective
The main objectives of this analysis are:

Calculate the monthly sales percentages for different avocado bag sizes across regions.
Compare the performance of small, large, and x-large bags over time.
Offer insights into which bag size is performing best in each region.

## SQL Query Breakdown
1. Number_Bags_Sold CTE
This Common Table Expression (CTE) aggregates the number of small, large, and x-large bags sold per region and month. It groups the data by formatted month and region, calculating total sales for each bag size.
2. Total_Sales CTE
This CTE calculates the total number of all bags (small, large, and x-large combined) sold per region and month. This will allow us to compute the percentage of each bag size later.
3. Final SELECT Statement
This section calculates the sales percentage of each bag size by dividing the number of bags sold (num_sold) by the total bags sold (total_sales), multiplying by 100 to get the percentage. The results are then rounded to the nearest whole number for easier readability.

## Results
The query will return the following columns:

date: The month of the sales (formatted as YYYY_MM).
region: The region where the sales occurred.
bag_size: The size of the bag (small, large, x-large).
sales_percentage: The percentage of total bags sold that each bag size represents.

## How to Use
Download the Avocado Prices Dataset from Kaggle.
Run the SQL query in BigQuery using the appropriate dataset.
Analyse the resulting sales percentages to see which bag sizes are most popular across regions and time periods.
Attribution
Please make sure to credit the original dataset:
This project uses data from Kaggle, licensed under the ODbL v1.0.

## Future Improvements
Visualisation of the sales percentage data to spot trends more easily.
Deeper analysis comparing organic vs conventional avocado types.
Extending the analysis to include price trends alongside bag size sales.
