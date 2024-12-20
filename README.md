# Drivers Data Analysis Report

## Project Overview
The aim of this project is to explore and analyze a dataset containing detailed information about drivers, including their age, city, years of experience, average rating, and active status. This data provides valuable insights into the profiles of drivers, offering opportunities to identify patterns and trends that could inform decision-making processes in areas such as driver recruitment, rating systems, and operational strategies.

Through various exploratory data analysis (EDA) techniques, we investigate the distribution of key variables, such as age and experience, and examine relationships between these factors and the drivers' average ratings. We also apply statistical methods to test hypotheses about the relationship between drivers' age and their ratings.

By analyzing the data visually and statistically, this project seeks to uncover meaningful insights about driver characteristics, assess the overall distribution of ratings and experience, and evaluate the effectiveness of certain factors in influencing driver performance and activity status. The findings from this project can be used to guide future strategies for driver management, performance evaluation, and workforce optimization.

## Data Source

The data that was used in this study is Drivers data posted on Kaggle, an online portal for community of data scientists. The dataset provides insights into drivers' performance and demographic characteristics, with key attributes such as the number of years of experience and the average ratings given to each driver. It also categorizes drivers as "Active" or "Inactive.". The data is free from missing values, ensuring its readiness for analysis. It is structured with a mix of numerical and categorical columns, allowing for various statistical tests and comparisons.

## Tools

The project utilized Python for various stages of data analysis, including data cleaning and preprocessing, exploratory data analysis (EDA), and A/B testing. Python's powerful libraries, such as Pandas, were employed to clean and preprocess the data, ensuring it was structured and free of errors or inconsistencies. For exploratory data analysis, Python libraries such as Numpy, Scipy, Matplotlib.pyplot and seaborn were used to generate summary statistics, visualize data distributions, and identify trends. Additionally, Hypothesis testing was conducted to compare the average ratings of drivers.

## Data Preparation
In this project, the dataset was thoroughly cleaned and preprocessed to ensure its quality before conducting any analysis. The following steps were performed as part of the data cleaning process:

#### 1. Checking for Duplicates:
We checked for duplicate records in the dataset using the duplicated() method. The result indicated that there are no duplicates in the dataset, confirming that each row represents a unique driver.

#### 2. Checking for Missing Values:
Missing values were checked using the isnull() method. The analysis revealed that there are no missing values in any of the columns, ensuring that the dataset is complete and ready for further analysis.

#### 3. Checking Data Types:
The data types of each column were verified using the dtypes method. All columns have the appropriate data types, ensuring that the dataset is properly structured for analysis. For example, numerical values (such as age, years of experience, and ratings) are correctly recognized as numerical data types.

#### 4. Dataset Information:
The info() method was used to gather an overview of the dataset, which confirmed that it contains 100 rows and 7 columns. All columns contain valid data, and the dataset is free from issues like incorrect data types or missing values.

#### 5. Shape of the Dataset:
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

## Data Analysis

The data analysis in this project involved a detailed examination of the drivers' dataset through both descriptive statistics and hypothesis testing. The key findings and conclusions are as follows:

Statistical Analysis:

A hypothesis test was conducted to evaluate whether drivers aged 40 and above have higher average ratings compared to those under 40. The null hypothesis proposed that older drivers would have higher ratings, while the alternative hypothesis suggested the opposite.
The results of the t-test showed a t-statistic of 2.13 and a p-value of 0.035, which is below the significance level of 0.05. This led to the rejection of the null hypothesis, suggesting that there is no significant difference in average ratings between drivers aged 40 and above and those below 40.
Key Insights:

The analysis revealed that while most drivers have high ratings, there is no direct evidence to suggest that older drivers consistently perform better in terms of ratings.
The distribution of experience years showed that many drivers have a relatively high level of experience, though the skewness suggests a prevalence of drivers with fewer years of experience.

## Findings

- Relationships Between Variables:

There is no significant correlation between age and years of experience, as confirmed by both the scatter plot and the heatmap. This suggests that older drivers do not necessarily have more years of experience and vice versa.
Other variables in the dataset also show low correlations, indicating that drivers' ratings, experience, and age are not strongly interdependent.

- Hypothesis Testing:

A hypothesis test comparing the average ratings of drivers aged 40 and above with those below 40 showed that there is no significant difference between the two groups. The null hypothesis, which suggested that older drivers would have higher ratings, was rejected based on the test results (t-statistic = 2.13, p-value = 0.035). This finding suggests that age does not significantly affect a driver's rating.


## Conclusion

The findings highlight that while drivers tend to have high ratings, age and experience do not appear to significantly impact their performance or ratings. These insights provide a better understanding of the drivers' profiles and can help guide future decisions related to driver management, performance assessments, and operational strategies. The lack of correlation between key variables also suggests that factors like age and experience may not be the most critical determinants of driver performance, opening the door to exploring other influencing factors in future analyses.

## Recommendations

#### 1. Explore Additional Factors Affecting Ratings:
Since there is no significant correlation between age, experience, and ratings, it would be valuable to explore other factors that might influence driver performance and ratings. These could include variables such as driving behavior, customer feedback, location, or work hours. Analyzing these factors could provide a more comprehensive understanding of what drives high ratings.

#### 2. Targeted Training for Inexperienced Drivers:
Given the left-skewed distribution of years of experience, with many drivers having fewer years of experience, it may be beneficial to implement targeted training programs for less experienced drivers. These programs could focus on improving driving skills and customer service, which could help boost ratings and overall performance.

#### 3. Investigate Inactive Drivers:
With 45% of the drivers being inactive, it could be useful to investigate the reasons behind their inactivity. Conducting surveys or interviews with inactive drivers may provide insights into factors such as job satisfaction, work-life balance, or performance issues. This information could help design strategies to re-engage inactive drivers or improve retention.

#### 4. Consider Age-Related Preferences in Driver Assignment:
Although the analysis did not show a significant correlation between age and ratings, other factors, such as preferences or customer demographics, might play a role in driver assignment. It might be useful to explore if certain age groups are preferred by specific types of customers or in particular regions, optimizing assignments based on these preferences.

#### 5. Implement a Continuous Feedback System:
Given the high concentration of drivers with ratings between 4.8 and 5.0, implementing a continuous feedback and performance tracking system could help maintain and improve the quality of service. Regular feedback could help drivers fine-tune their performance, leading to better ratings and higher customer satisfaction over time.
