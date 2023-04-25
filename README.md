# MATH4581 Project
For this project, the aim is to determine how different attributes can correlate with life expectancy in different countries. I aim to determine which of the many health factors has the highest correlation with life expectancy. After obtaining the three (3) factors with the highest correlation, I will perform linear regression, and determine if the line of best fit is statistically significant. Afterwards, I will determine the confidence interval. 
## Steps
First, I imported the dataset aquired from Kaggle.com. The dataset contains life expectancy values from the WHO along with othetr factors that may influence a country's life expectancy. 

After cleaning and preparing the data, I determined the correlation value for each factor with respect to life expectancy. 
!["Correlation of each feature](correlation.png)

Afterwards, I determined that the three factors with the highest (absolute) correlation factors were adult morality, income composition of resources, and schooling. 
These factors are defined below. 
- Adult morality - probability of dying between 15 and 60 years per 1000 population
- Income Composition of Resources - Human Development Index in terms of income composition of resources (index ranging from 0 to 1)
- Schooling - Number of years of Schooling(years)

After obtaining the three health factors with the highest correlation factor, I used Scipy's LinearRegression library (linregress) to calculate the intercept, slope, and p-value of the regression line for each factor.

## Results
| Health Factor | Slope | Intercept | P-Value | Linear Regression Test Conclusion
|---|---|---|---|---|
| Schooling | 2.10 | 44.11 | 0.00 | Reject null hypithesis |
| 
