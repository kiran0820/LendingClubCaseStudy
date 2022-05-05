# Lending Club Case Study
> Lending Club is a consumer finance company which specialises in lending various types of loans to urban customers. Their aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.

## Table of Contents
* [Technologies Used](#technologies-used)
* [Data Understanding](#data-understanding)
* [Data Cleaning](#data-cleaning)
* [Data Analysis](#data-analysis)


## Technologies Used
- Python 7.29.0 to use chart library
- Seaborn library for chart representation
- Plotly library for bar chart 

## Data Understanding
- The objectives of data understanding are:
	- Understand the attributes of the data.
	- Summarize the data by identifying key characteristics, such as data volume and total number of variables in the data.
	- Understand the problems with the data, such as missing values, inaccuracies, and outliers.
	- Visualize the data to validate the key characteristics of the data or unearth problems with the summary statistics.
	
## Data Cleaning
- If we look into CSV, we will find out that:
	- This dataset contains 39717 rows and 111 columns. Out of these 111 columns, many columns have null values in majority.
	- Columns with null values must be dropped. 
	- Categorize the columns into 3 category i.e. "Customer's Basic Information", "Loan Information" , and "Customer Behaviour variables".
	- As "Customer Behaviour variables" doesnot add any input to find out the factor behing being defaulters, so we can eliminate these columns.
	- Also, there are some columns which are having single value through out. So we must eliminate those columns too.
	- As we are working to find out defaulters driving factors, so we can drop out the rows having value as "Current" for "Loan Status" columns.
	- We can too remove the unique identifier whose presence does not have much influence on data.
	- The columns [‘issue_d’] which are datetime columns are further divided into month and year by using pandas datetime module.

## Data Analysis
- We have done following analysis to find out the driving factors for defaulters:
	- Univariate Analysis
	- Segemented Univariate Analysis
	- Bivaraiate/Multivariate Analysis



## Contact
Created by @kiran0820 - feel free to contact me!