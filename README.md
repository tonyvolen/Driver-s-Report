# Drivers Data Analysis Report

## Table of Contents

- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Preparations](#data-preparations)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analsis)
- [Findings](#findings)
- [Conclusion](#conclusion)
- [Recommendations](#recommendations)
## Project Overview


The aim of this project is to explore and analyze a dataset containing detailed information about drivers, including their age, city, years of experience, average rating, and active status. This data provides valuable insights into the profiles of drivers, offering opportunities to identify patterns and trends that could inform decision-making processes in areas such as driver recruitment, rating systems, and operational strategies.

Through various exploratory data analysis (EDA) techniques, we investigate the distribution of key variables, such as age and experience, and examine relationships between these factors and the drivers' average ratings. We also apply statistical methods to test hypotheses about the relationship between drivers' age and their ratings.

By analyzing the data visually and statistically, this project seeks to uncover meaningful insights about driver characteristics, assess the overall distribution of ratings and experience, and evaluate the effectiveness of certain factors in influencing driver performance and activity status. The findings from this project can be used to guide future strategies for driver management, performance evaluation, and workforce optimization.

## Data Source


The data that was used in this study is Drivers data posted on Kaggle, an online portal for community of data scientists. The dataset provides insights into drivers' performance and demographic characteristics, with key attributes such as the number of years of experience and the average ratings given to each driver. It also categorizes drivers as "Active" or "Inactive.". The data is structured with a mix of numerical and categorical columns, allowing for various statistical tests and comparisons.

## Tools


The project utilized Python for various stages of data analysis, including data cleaning and preprocessing, exploratory data analysis (EDA), and hypothesis testing. Python's powerful libraries, such as Pandas, were employed to clean and preprocess the data, ensuring it was structured and free of errors or inconsistencies. For exploratory data analysis, Python libraries such as Numpy, Scipy, Matplotlib.pyplot and seaborn were used to generate summary statistics, visualize data distributions, and identify trends. Additionally, Hypothesis testing was conducted to compare the average ratings of drivers.

## Data Preparation


In this project, the dataset was thoroughly cleaned and preprocessed to ensure its quality before conducting any analysis. The following steps were performed as part of the data cleaning process:

#### 1. Checking for Duplicates:
We checked for duplicate records in the dataset and the result indicated that there are no duplicates in the dataset, confirming that each row represents a unique driver.

#### 2. Checking for Missing Values:
Missing values were checked and the analysis revealed that there are no missing values in any of the columns, ensuring that the dataset is complete and ready for further analysis.

#### 3. Checking Data Types:
The data types of each column were verified and all columns had the appropriate data types, ensuring that the dataset is properly structured for analysis.

#### 4. Dataset Information:
We gathered an overview of the dataset, which confirmed that it contains 100 rows and 7 columns. All columns contain valid data, and the dataset is free from issues like incorrect data types or missing values.

#### 5. Shape of the Dataset:
The dataset's shape was checked using the shape method, which confirmed that it contains 100 rows and 7 columns, providing a manageable size for analysis.

## Exploratory Data Analysis


In this project, the exploratory data analysis was performed to better understand the dataset and uncover meaningful patterns and insights. The following key steps were taken during the EDA process:

#### 1. Distribution of Driver’s Age:
A QQ plot of the drivers' age revealed that the data is not normally distributed, as the points did not align with the diagonal line. This suggests that the distribution of ages does not follow a typical bell curve.

The QQ plot below shows the distribution of driver's age


![image](https://github.com/user-attachments/assets/eb4cfaab-c0c9-49a0-b491-b6bfb792ada1)


#### 2. Years of Experience:
Years of Experience  provides insights into the drivers' performance and how experience might influence their Average Rating or Active Status.

The box plot for years of experience showed a left-skewed distribution, indicating that a larger number of drivers have fewer years of experience. Additionally, the plot did not reveal any outliers, suggesting that the data on experience is relatively consistent.

The box plot below visualizes the distribution of drivers’ years of experience across the dataset



![image](https://github.com/user-attachments/assets/35c3cb0f-b410-4df1-8409-7132b7b44813)


#### 3. Average Rating Distribution:
In this dataset, most drivers have high average ratings, with many ratings clustered between 4.8 and 5.0, suggesting that the drivers are generally well-regarded by their customers.

The Histogram below visualizes the distribution of drivers’  average rating across the dataset



![image](https://github.com/user-attachments/assets/197392ce-882a-41b9-a67b-697c26294cdb)


#### - Skeweness
The skewness of the average ratings is negative, suggesting that the data is skewed to the left (with more drivers having ratings on the higher end).
#### - Kurtosis
The kurtosis value is also negative, indicating that the distribution is platykurtic, meaning it has a short tail and is flatter than a normal distribution.



#### 4.Active Status Distribution:
A pie chart displayed the proportion of active versus inactive drivers, revealing that 55% of the drivers are active, while 45% are inactive, providing insight into the current activity levels within the dataset.

The below pie chart shows the distribution of drivers’ active status


![image](https://github.com/user-attachments/assets/33e056c3-cacc-4148-b4a3-1b38537a10a4)


## Data Analysis


The data analysis in this project involved a detailed examination of the drivers' dataset through both descriptive statistics and hypothesis testing.

#### Descriptive Statistics

##### - Scatter Plot & Correlation:
The scatter plot between age and years of experience revealed no clear linear relationship between these two variables. This suggests that there is no direct correlation between a driver’s age and the number of years of experience they have.

The scatter plot below shows the relationship between drivers’ years of experience and their Ages.


![image](https://github.com/user-attachments/assets/c02a7bb9-b81b-49ce-9954-825723b3ea8a)

The heatmap further confirmed that there is a low correlation among the various variables in the dataset, indicating that none of the features are strongly related to one another.

The heat map below show correlation between the numerical variables of the drivers’ dataset.


![image](https://github.com/user-attachments/assets/eec9f5df-72f2-4113-bc53-741f60d2a5a0)

#### - Hypothesis Testing:

A hypothesis test was conducted to evaluate whether drivers aged 40 and above have higher average ratings compared to those under 40. 

- Null hypothesis: Drivers of age 40 and above have a high Average rating compared to drivers below 40 years.
- Alternative hypothesis:  Drivers of age 40 and above do not have high average rating compared to drivers below 40 years
  


## Findings


- Relationships Between Variables:

There is no significant correlation between age and years of experience, as confirmed by both the scatter plot and the heatmap. This suggests that older drivers do not necessarily have more years of experience and vice versa.
Other variables in the dataset also show low correlations, indicating that drivers' ratings, experience, and age are not strongly interdependent.

- Hypothesis Testing:

The results of the t-test showed a t-statistic of 2.13 and a p-value of 0.035, which is below the significance level of 0.05. This led to the rejection of the null hypothesis, suggesting that there is no significant difference in average ratings between drivers aged 40 and above and those below 40.

The analysis revealed that while most drivers have high ratings, there is no direct evidence to suggest that older drivers consistently perform better in terms of ratings.
The distribution of experience years showed that many drivers have a relatively high level of experience, though the skewness suggests a prevalence of drivers with fewer years of experience.

## Conclusion


The findings highlight that while drivers tend to have high ratings, age and experience do not appear to significantly impact their performance or ratings. These insights provide a better understanding of the drivers' profiles and can help guide future decisions related to driver management, performance assessments, and operational strategies. The lack of correlation between key variables also suggests that factors like age and experience may not be the most critical determinants of driver performance, opening the door to exploring other influencing factors in future analyses.

## Recommendations


1. Explore Additional Factors Affecting Ratings:
Since there is no significant correlation between age, experience, and ratings, it would be valuable to explore other factors that might influence driver performance and ratings.

2. Targeted Training for Inexperienced Drivers:
Given the left-skewed distribution of years of experience, with many drivers having fewer years of experience, it may be beneficial to implement targeted training programs for less experienced drivers.

3. Investigate Inactive Drivers:
 Conducting surveys or interviews with inactive drivers may provide insights into factors such as job satisfaction, work-life balance, or performance issues. This information could help design strategies to re-engage inactive drivers or improve retention.

4. Consider Age-Related Preferences in Driver Assignment:
Although the analysis did not show a significant correlation between age and ratings, other factors, such as preferences or customer demographics, might play a role in driver assignment.

5. Implement a Continuous Feedback System:
Given the high concentration of drivers with ratings between 4.8 and 5.0, implementing a continuous feedback and performance tracking system could help maintain and improve the quality of service.
