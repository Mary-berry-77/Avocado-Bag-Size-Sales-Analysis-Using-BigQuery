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

## Analysis 1: Sales Percentage Calculation with Grouping
SQL Query
This query calculates the sales percentage of each bag size based on the total bags sold. It categorizes the results into ranges for better insight.

## Analysis 2: Bag Size Sales Percentage Ranges
SQL Query
This query analyzes sales percentages and categorizes the results into defined ranges (e.g., "over 90%", "60-90%", "NO SALES"). This provides a clearer picture of sales performance for each bag size.

## Results
Both queries return insights into avocado sales by bag size, allowing for a comparative analysis of performance:

Analysis 1 provides a direct sales percentage for each bag size.
Analysis 2 categorizes the sales performance into ranges, highlighting zero sales situations for clearer reporting..

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
