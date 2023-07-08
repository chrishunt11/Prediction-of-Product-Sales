![bigmart](https://github.com/chrishunt11/Prediction-of-Product-Sales/assets/123383359/998a2af5-0f2c-4a58-b68e-1dd392901142)


# Production Sales and Insights
## Analyzing Product Sales 

**Author**: Christopher Hunt

### Business problem:

A problem retailers often run into is how to continually increase their sales. Within this problem there are subproblems they need to focus on. One is to figure out which products are worth selling; another is to figure out which outlets play a crucial role in increasing sales. There are many factors that come into play when deciding what to sell and where to sell it.

### Data Source:

Big Mart Sales Prediction: https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/

For this dataset there were 8523 rows and 12 columns

### Data Dictionary
<p align = "center"> 
  <img width="429" alt="Data Dictionary" src="https://github.com/chrishunt11/Prediction-of-Product-Sales/assets/123383359/06c0f6b5-b1be-4a6d-8712-6cff3262a07c">
</p>

### To prepare this data, the data was cleaned, and the following processes were performed:

#### Exploratory Data Analysis

- During the exploratory data analysis, a histogram and a boxplot was visualized for Outlet Sales, MRP, Visibility, Outlet Type, and Outlet Location.
- Also, countplots were visualized for the Outlet location and Type.
- This gave good baseline for all the Sales of the Products and the count for the Location and Type.

![Visibilitypng](https://github.com/chrishunt11/Prediction-of-Product-Sales/assets/123383359/74f27d5c-bcf8-4361-b380-8a585a00707d)

This visual shows that the majority of the products have a visibility percentage of about 3 percent.

#### Explanitory Data Analysis

- During the Explanitory data analysis, a boxplot and histogram was visualized for each numeric datatype column.
- Also, a numerous barplots are visualized to get a better understanding of which outlet type and size have the most sales.
- This gave a good baseline for all of the numeric and caegorical columns for univariate and multivarite EDA.


![Mrp-OutletSales](https://github.com/chrishunt11/Prediction-of-Product-Sales/assets/123383359/94e0aeef-f97a-4c0e-8ce0-5dd8bee14070)


This visual shows that the greater the MRP price the greater the Outlet Sales.


![avg-sale-item](https://github.com/chrishunt11/Prediction-of-Product-Sales/assets/123383359/44733357-7ff1-404b-85ed-772a71817a26)


The top five highest earning sales per item type are as follows:
- Starchy Foods:            `$2,374.33`
- Seafood:                  `$2,326.07`
- Fruits and Vegetables:    `$2,289.01`
- Snack Foods:              `$2,277.32`
- Household:                `$2,258.78`

The bottom five highest earning sales per item types are as follows:
- Breakfast:                `$2,111.81`
- Health and Hygiene:       `$2,010.00`
- Soft Drinks:              `$2,006.51`
- Baking Goods:             `$1,952.97`
- Others:                   `$1,926.14`



![sales-outlet-size](https://github.com/chrishunt11/Prediction-of-Product-Sales/assets/123383359/4369bdbe-1c14-4fd0-8bea-b290c969de04)


This barplot shows that the most sales were at Medium sized stores.


In order, the outlet sales per outlet size are as follows:
- Medium:          `$2,681.60`
- High:            `$2,299.00`
- Small:           `$1,912.15`


![sales-outlet-type](https://github.com/chrishunt11/Prediction-of-Product-Sales/assets/123383359/093ee71e-b17c-4816-8624-d49f8cc519fc)


This barplot shows that majority of the outlet sales were at Supermarket type 3.


In order, the outlet sales per outlet type are as follows:
- Supermarket Type3:	    `$3,694.04`
- Supermarket Type1:	    `$2,316.18`
- Supermarket Type2:	    `$1,995.50`
- Grocery Store:	        `$339.83`

 ### Maching Learning Using the Following Models:
    - Linear Regression Model
    - Bagged Tree Regressor Model
    - Tuned Bagged Tree Regressor Model
    - Random Forest Regressor Model
    - Tuned Random Forest Regressor Model

## Models Evaluated & Results

- Linear Regression Model (Testing Set):
  - R^2 = 0.570
  - MAE = 802.048
  - MSE = 1,186,964.271
  - RMSE = 1,089.479

- Bagged Tree Regressor Model (Testing Set):
  - R^2 = 0.526
  - MAE = 795.198
  - MSE = 1,306,771.261
  - RMSE = 1,143.141

- Tuned Bagged Tree Regressor Model (Testing Set):
  - R^2 = 0.578
  - MAE = 756.837
  - MSE = 1,163,912.604
  - RMSE = 1,078.848 

- Random Forest Model (Testing Set):
  - R^2 = 0.554
  - MAE = 773.627
  - MSE = 1,229,857.716
  - RMSE = 1,108.990

- Tuned Random Forest Model (Testing Set):
  - R^2 = 0.595
  - MAE = 736.676
  - MSE = 1,116,454.429
  - RMSE = 1,056.624

- The Final Model Chosen was a 'Random Forest Regressor Model' with the n_estimators tuned to 150.
- For the testing model '59.5%' of the variance in y was explained by X.
- The Mean Absolute Error was off by about '$736.68'
- The Mean Squared Error was '$1,116,454.43'.
- The Root Mean Squared Error had a calculation of '$1,056.62'

Using this model to make predictions about what Products to sell at which Outlet Location and Type would not be very reliable. After reviewing the regression metrics on how well the model performed, there is a disparity between the R^2 score.

## Recommendations:

- There appears to be a moderate correlation between Item MRP and Item Sales. If a retailor were to look to increase their Sales, one thing they could try doing is increase the Item MRP.

Model Performace 
- Overall, the best model is definitely the tuned Random Forest Regressor Model. The model is a little over fit, but by far it outperformed the linear regression model.


## Limitations & Next Steps

From here, a student could use the insights from the visuals on how to increase the Sales and could look for more correlations within the data.

### For further information


For any additional questions, please contact:
- Christopher Hunt Jr.
- cjhunt592.1@gmail.com
