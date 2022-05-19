# Sample project: Time-series analysis

### Today I got a note from Tim, the store manager for the downtown branch.

> Jacob-
> 
> We have daily sales data for the last four years, and we'd love some insight into how to schedule our salespeople. I certainly can't find any pattern in the data, but maybe you can with your 'machine learning' stuff? Let me know if you have any insights.
> 
> Thanks.
> 
> -Tim

## 🎯 Goals
* Explore the dataset
* If possible, create a model which can predict store sales to inform staffing decisions
* Plot the sales predictions against the actual sales in the test set

## 🏗 Dependencies
* Python 3.9.7
* matplotlib.pyplot
* matplotlib.ticker
* numpy
* pandas
* seaborn
* holiday from pandas.tseries
* RandomForestRegressor from sklearn.ensemble
* permutation_importance from sklearn.inspection
* acf, pacf from statsmodels.tsa.stattools
* plot_acf, plot_pacf from statsmodels.graphics.tsaplots

## 📂 Data
[CSV in repository](https://github.com/JacobTews/simple_time_series/blob/6accaec676f46096145079196a7b48afc831506b/store_sales_small.csv)

(Original source unknown)

## 💡 Insights
* Salaries for tech roles **peak mid-career (age 35-44)**, likely because some of those in higher age brackets have moved into leadership positions and no longer identify as software engineers/developers.
* Salaries are notably **higher for those paid in $USD** than elsewhere.
* Salaries are particularly **low for those in the United Kingdom**.
<br/><br/>
![salary bar graph](https://github.com/JacobTews/preprocessing_and_eda/blob/main/insights/compensation_visual.png?raw=true)

## 🛠 Want to dig into my code?
Here's the [notebook](https://github.com/JacobTews/simple_time_series/blob/6accaec676f46096145079196a7b48afc831506b/time_series_analysis.ipynb) for your perusal, fully annotated.
