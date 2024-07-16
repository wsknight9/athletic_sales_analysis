# athletic_sales_analysis
# Module 5 Challenge
# Background
# Analyze sales data to gain insights into which cities in the U.S. have sold the most athletic wear over two years. Next, determine which retailers had the greatest total sales for athletic wear, and which retailers sold the most women's athletic footwear. Finally, determine which day and week had the highest sales for women's athletic footwear.
#
# Before starting the assignment, be sure to complete the following steps:
#
# Create a new repository for this project called athletic_sales_analysis. Do not add this homework assignment to an existing repository.
#
# Clone the new repository to your computer.
#
# Push these changes to GitHub or GitLab.
#
# Files
# Download the following files to get started:
# https://static.bc-edx.com/ai/ail-v-1-0/m5/lms/starter/M5_Starter_Code.zip
#
# Challenge Instructions
# The starter code provided includes all the steps necessary to complete this challenge.
#
# Combine and Clean the Data
# Import the two CSV files, athletic_sales_2020.csv and athletic_sales_2021.csv, and read them into DataFrames.
#
# Check that the columns in the two DataFrames have similar names and data types.
#
# Combine the two DataFrames by the rows using an inner join, and reset the index.
# HINT
# Read over the instructions to determine if you should use concat, join, or merge.
# After combining the DataFrames, do the following:

# Check if there are any null values.

# Check each column’s data type.

# Convert the "invoice_date" column to a datetime data type.

# Confirm that the data type has been changed.

# Determine which Region Sold the Most Products
# Use either the groupby or pivot_table function to create a multi-index DataFrame with the "region", "state", and "city" columns.

# Rename the aggregated column to reflect the aggregation of the data in the column.

# Sort the results in descending order to show the top five regions, including the state and city that have the greatest number of products sold. Your final table should look like the following image:

# The top five regions with their states and cities that have the greatest number of products sold.
# Determine which Region had the Most Sales
# Use either the groupby or pivot_table function to create a multi-index DataFrame with the "region", "state", and "city" columns.

# Rename the aggregated column to reflect the aggregation of the data in the column.

# Sort the results in descending order to show the top five regions, including the state and city that generated the most sales. Your final table should look like the following image:

# The top five regions with their states and cities that generated the most sales.
# Determine which Retailer had the Most Sales
# Use either the groupby or pivot_table function to create a multi-index DataFrame with the "retailer", "region", "state", and "city" columns.

# Rename the aggregated column to reflect the aggregation of the data in the column.

# Sort the results in descending order to show the top five retailers along with their region, state, and city that generated the most sales. Your final table should look like the following image:

# The top five retailers along with their region, state, and city that have the greatest average price for the products ordered.
# Determine which Retailer Sold the Most Women's Athletic Footwear
# Filter the combined DataFrame to create a DataFrame with only women's athletic footwear sales data.

# HINT
# Use df[df["column_name"].str.contains("<value>")] or df.loc[(df["column_name"] =="<value>")].

# Use either the groupby or pivot_table function to create a multi-index DataFrame with the "retailer", "region", "state", and "city" columns.

# Rename the aggregated column to reflect the aggregation of the data in the column.

# Sort the results in descending order to show the top five retailers along with their region, state, and city that sold the most women's athletic footwear. Your final table should look like the following image:

# The top five retailers along with their region, state, and city that sold the most women's athletic footwear.
# Determine the Day with the Most Women's Athletic Footwear Sales
# Create a pivot table with the "invoice_date" column as the index and the "total_sales" column as the values parameter.

# Rename the aggregated column to reflect the aggregation of the data in the column.

# Apply the resample function to the pivot table, place the data into daily bins, and get the total sales for each day.

# Sort the resampled DataFrame in descending order to show the top 10 days that generated the most women's athletic footwear sales. Your final table should look like the following image:

# The top 10 days that generated the most women's athletic footwear sales.
## Determine the Week with the Most Women's Athletic Footwear Sales
# Apply resample to the pivot table above, place the data into weekly bins, and get the total sales for each week.

# Sort the resampled DataFrame in descending order to show the top 10 weeks that generated the most women's athletic footwear sales. Your final table should look like the following image:

# The top 10 weeks that generated the most women's athletic footwear sales.
# Submission
# To submit your Challenge assignment, click Submit, and then provide the URL of your GitHub repository for grading.
# References
# Followed Class Activities for basic code
# Stack Overflow website
# Sales Product Data. Available: https://www.kaggle.com/datasets/knightbearr/sales-product-dataLinks to an external site.
# The sales product data above was modified by edX Boot Camps LLC, and is intended for educational purposes only.
