# life-expectancy-regression-analysis

# What Best Predicts Life Expectancy?

### A Linear Regression Analysis Using Global Health and Economic Data

This project analyzes global demographic and economic data to determine which variables best predict life expectancy using linear regression models.

The project combines datasets containing:

* GDP per capita
* Population
* Fertility rate
* Child mortality rate
* Life expectancy

The datasets were cleaned and merged using country code and year, resulting in a final dataset containing 1184 observations from 74 countries between 2000–2015.

---

# Objective

The goal of this project was to determine which variables most strongly predict life expectancy and compare their predictive performance using regression analysis.

Before training the models, the hypothesis was that GDP per capita and poverty-related variables would be the strongest predictors of life expectancy.

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

---

# Model Creation

The dataset was divided into:

* 80% training data
* 20% testing data

using Python’s `train_test_split` function from scikit-learn.

Multiple linear regression models were trained using different combinations of variables. Model performance was evaluated using:

* R² Score
* RMSE (Root Mean Squared Error)

---

# Results

| Variables Tested     | R² Score | RMSE |
| -------------------- | -------- | ---- |
| Population Only      | ~0.02    | ~7.9 |
| GDP Per Capita Only  | 0.48     | 5.72 |
| Fertility Only       | 0.73     | 4.13 |
| Child Mortality Only | 0.83     | 3.30 |
| Full Model           | 0.86     | 3.01 |

The results showed that child mortality was the strongest individual predictor of life expectancy, while GDP per capita had a weaker relationship than expected.

The final regression model explained approximately 86% of the variation in life expectancy with an average prediction error of about 3 years.

---

# Visualizations

The project includes:

* Scatterplots comparing each variable against life expectancy
* Model comparison results
* Actual vs Predicted life expectancy plots

---

# Key Takeaways

* Child mortality was the strongest predictor of life expectancy
* Population alone had almost no predictive power
* Healthcare-related variables appeared more predictive than economic variables alone
* Linear regression successfully modeled global life expectancy trends
