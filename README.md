Car Sales Analysis


Project Overview

This project performs an end-to-end exploratory data analysis (EDA) of a second-hand car sales dataset. The notebook walks through importing, cleaning, and analyzing 50,000 records of used cars, focusing on price distribution, mileage trends, manufacturer comparisons, and relationships between features such as engine size and year of manufacture.


Dataset Details

File: car_sales_data.csv
Shape: 50,000 rows × 7 columns
Columns:
Manufacturer – Brand of the car (e.g., Ford, Toyota, Porsche)
Model – Model name
Engine size – Engine capacity in liters
Fuel type – Petrol, Diesel, Hybrid, etc.
Year of manufacture – Year produced
Mileage – Kilometers driven
Price – Listed price
The dataset was checked for missing values and duplicates, and 12 duplicate rows were removed to ensure clean analysis.


Libraries Used

pandas and numpy – Data handling and computation
matplotlib and seaborn – Distribution plots, histograms, boxplots
plotly.express and graph_objects – Interactive charts for deeper exploration


Analysis Performed

1. Data Inspection

Used df.info() and df.describe() to review data types and summary statistics.

Verified non-null counts for all columns.



2. Data Cleaning

Removed duplicate rows using df.duplicated().sum().

Checked for missing values with df.isna().sum().



3. Univariate Analysis

Price distribution visualized using seaborn histplot.

Mileage distribution visualized to show typical driving distance patterns.

Engine size distribution analyzed to check concentration of engine types.



4. Bivariate Analysis

Price vs. engine size scatter plots and boxplots revealed a positive correlation.

Price vs. year of manufacture identified depreciation trends, with newer cars costing more.

Price vs. mileage showed a negative relationship.

Grouped average price per manufacturer to highlight high-value brands.



5. Fuel Type Analysis
   
Bar plot of fuel type counts showed the distribution between Petrol, Diesel, Hybrid, and others.

Average price comparison across fuel types revealed differences in market value.



6. Interactive Visualizations

Interactive histograms and scatter plots created using Plotly to make data exploration easier.



Key Observations

Prices are right-skewed, with most cars in lower price ranges and a few expensive outliers.

Mileage and price are inversely related, meaning cars with higher mileage typically sell for less.

Engine size has a positive influence on price, with larger engines usually commanding higher value.

Certain manufacturers such as Porsche and BMW dominate the higher price bracket.

Older cars show sharp price depreciation after about 10 to 15 years.
