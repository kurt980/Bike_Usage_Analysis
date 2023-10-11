# Bike_Usage_Analysis
This is a class project I did ealier this year. The data is bike usage data in a 2-year span. Key features include date, time, weather-related variables. I used multiple modeling techniques to explore, examine and predict this data. 

## Content
### Exploratory analysis
The exploratory analysis consists of visualization between bike usage and day of the week, as well as weather variables. I also did a correlation analysis between variables

### Linear Regression
The linear regression serves as a indicator of data distribution. It is obvious that the data does not meet the assumptions for linear regression. Log-transform on the response is done, which increases most metrics. A cubic polynomial is done on the features which also significantly improves accuracy. This shows that the response has a non-linear relationship with the predictors, and a non-gaussian distribution, which is obvious because bike usage cannot go to zero.

### Generalized Regression Models
I have applied multiple GLMs with different distribution. For example, poisson model is assumed and improves performance. But poisson distribution has to satisfy the dispersion condition which means the mean has to equal to variance. The data obviously does not meet this condition so I used negative-binomial as the underlying distribution. The NB regression is by far the best regression model.

### Non-parametric Models
XGBoost and Random Forest provide much better performance for this dataset. But I really enjoy exploring the nature of the data using regression models.
