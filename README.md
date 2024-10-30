# cpi_case_study_project
CPI Inflation Case Study
Overview
This case study analyzes the impact of COVID-19 on inflation using Excel. The analysis includes identifying the biggest contributor to the food category, determining the year and month with the highest inflation, and analyzing the correlation between fuel prices and other categories.

Data Sources
CPI Data: Historical CPI data (e.g., cpi_data.xlsx).
COVID-19 Impact Data: Data on COVID-19 impact on inflation (e.g., covid_impact_data.xlsx).
Food Category Data: Data on food sub-categories (e.g., food_data.xlsx).
Fuel and Other Categories Data: Data on fuel and other CPI categories (e.g., fuel_data.xlsx, other_categories_data.xlsx).
Data Processing and Analysis in Excel
1. Impact of COVID-19 on Inflation
Load Data:

Open cpi_data.xlsx and covid_impact_data.xlsx in Excel.
Merge the datasets using common date fields.
Calculate Inflation Rate:

Create a new column for Inflation Rate in the merged dataset:
= (CPI_Current - CPI_Previous) / CPI_Previous * 100
Analyze Impact:

Use PivotTables to analyze average Inflation Rate and COVID-19 impact by date.
2. Biggest Contributor to Food Bucket
Load Food Data:

Open food_data.xlsx in Excel.
Aggregate Food Sub-Categories:

Use the SUM function to aggregate contributions by sub-category:
= SUMIFS(Contribution, SubCategory, "SubCategory_Name")
Identify Top Contributor:

Use sorting or PivotTables to find the sub-category with the highest contribution.
3. Year and Month with Most Inflation
Prepare Data:

Extract year and month from the date in the cpi_data.xlsx file:
= YEAR(Date)
= MONTH(Date)
Aggregate Inflation Rates:

Use PivotTables to calculate average inflation rates by year and month.
Find Maximum Inflation:

Sort the PivotTable results to identify the year and month with the highest average inflation rate.
4. Correlation Between Fuel and Other Categories
Load Data:

Open fuel_data.xlsx and other_categories_data.xlsx in Excel.
Merge these datasets on the date field.
Calculate Correlation:

Use the CORREL function to find correlations between fuel prices and other categories:
= CORREL(Fuel_Range, Other_Category_Range)
Findings
Impact of COVID-19 on Inflation:

Analyzed changes in inflation rates during different phases of the COVID-19 pandemic.
Biggest Contributor to Food Bucket:

Identified the food sub-category with the highest contribution to inflation.
Year and Month with Most Inflation:

Determined the year and month with the highest inflation rates.
Correlation Analysis:

Examined the correlation between fuel prices and other CPI categories.
Visualizations
Trend Charts: Created to show inflation rates over time.
Bar Charts: Display contributions by food sub-categories.
Correlation Matrix: Visualized correlations between fuel and other categories.
Getting Started
Open Excel Files:

Load the relevant datasets in Excel.
Perform Analysis:

Follow the steps outlined above for data processing and analysis.
Create Visualizations:

Use Excel's charting tools to create visual representations of your findings.
Future Work
Expand Analysis: Consider additional factors influencing inflation, such as geopolitical events.
Refine Models: Develop more detailed models to predict inflation trends.
