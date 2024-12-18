# Drivers Data Analysis Report

## Project Overview
The aim of this project is to explore and analyze a dataset containing detailed information about drivers, including their age, city, years of experience, average rating, and active status. This data provides valuable insights into the profiles of drivers, offering opportunities to identify patterns and trends that could inform decision-making processes in areas such as driver recruitment, rating systems, and operational strategies.

Through various exploratory data analysis (EDA) techniques, we investigate the distribution of key variables, such as age and experience, and examine relationships between these factors and the drivers' average ratings. We also apply statistical methods to test hypotheses about the relationship between drivers' age and their ratings.

By analyzing the data visually and statistically, this project seeks to uncover meaningful insights about driver characteristics, assess the overall distribution of ratings and experience, and evaluate the effectiveness of certain factors in influencing driver performance and activity status. The findings from this project can be used to guide future strategies for driver management, performance evaluation, and workforce optimization.

## Data Source

## Tools


## Data Preparation
In this project, the dataset was thoroughly cleaned and preprocessed to ensure its quality before conducting any analysis. The following steps were performed as part of the data cleaning process:

1. Checking for Duplicates:
We checked for duplicate records in the dataset using the duplicated() method. The result indicated that there are no duplicates in the dataset, confirming that each row represents a unique driver.

2. Checking for Missing Values:
Missing values were checked using the isnull() method. The analysis revealed that there are no missing values in any of the columns, ensuring that the dataset is complete and ready for further analysis.

3. Checking Data Types:
The data types of each column were verified using the dtypes method. All columns have the appropriate data types, ensuring that the dataset is properly structured for analysis. For example, numerical values (such as age, years of experience, and ratings) are correctly recognized as numerical data types.

4. Dataset Information:
The info() method was used to gather an overview of the dataset, which confirmed that it contains 100 rows and 7 columns. All columns contain valid data, and the dataset is free from issues like incorrect data types or missing values.

5. Shape of the Dataset:
The dataset's shape was checked using the shape method, which confirmed that it contains 100 rows and 7 columns, providing a manageable size for analysis.

## Exploratory Data Analysis

In this project, the exploratory data analysis (EDA) was performed to better understand the dataset and uncover meaningful patterns and insights. The following key steps were taken during the EDA process:

#### 1. Distribution of Driver’s Age:
A QQ plot of the drivers' age revealed that the data is not normally distributed, as the points did not align with the diagonal line. This suggests that the distribution of ages does not follow a typical bell curve.

#### 2. Years of Experience:
The box plot for years of experience showed a left-skewed distribution, indicating that a larger number of drivers have fewer years of experience. Additionally, the plot did not reveal any outliers, suggesting that the data on experience is relatively consistent.

#### 3. Average Rating Distribution:
The histogram and KDE (Kernel Density Estimate) of the average ratings indicated that most drivers have ratings between 4.8 and 5.0, with a non-symmetric and non-bell-shaped distribution. This indicates that the ratings data is not normally distributed.

#### - Skeweness
The skewness of the average ratings is negative, suggesting that the data is skewed to the left (with more drivers having ratings on the higher end).
#### - Kurtosis
The kurtosis value is also negative, indicating that the distribution is platykurtic, meaning it has a short tail and is flatter than a normal distribution.

#### 4. Scatter Plot & Correlation:
The scatter plot between age and years of experience revealed no clear linear relationship between these two variables. This suggests that there is no direct correlation between a driver’s age and the number of years of experience they have.

The heatmap further confirmed that there is a low correlation among the various variables in the dataset, indicating that none of the features are strongly related to one another.

#### 5.Active Status Distribution:
A pie chart displayed the proportion of active versus inactive drivers, revealing that 55% of the drivers are active, while 45% are inactive, providing insight into the current activity levels within the dataset.
