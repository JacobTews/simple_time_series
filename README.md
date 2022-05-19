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
* If possible, create a model which can predict store sales
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
[CSV in repository](https://github.com/JacobTews/preprocessing_and_eda/blob/main/data/Ask%20A%20Manager%20Salary%20Survey%202021%20(Responses)%20-%20Form%20Responses%201.csv)

[Original source](https://www.askamanager.org/2021/05/look-at-24000-peoples-real-life-salaries.html)
* N.B. - While the dataset is substantial, the responses for any one specific category (with a few exceptions) are limited, so general conclusions will require further study.

## 💡 Insights
* Salaries for tech roles **peak mid-career (age 35-44)**, likely because some of those in higher age brackets have moved into leadership positions and no longer identify as software engineers/developers.
* Salaries are notably **higher for those paid in $USD** than elsewhere.
* Salaries are particularly **low for those in the United Kingdom**.
<br/><br/>
![salary bar graph](https://github.com/JacobTews/preprocessing_and_eda/blob/main/insights/compensation_visual.png?raw=true)

## 🛠 Want to dig into my code?
Here's the [notebook](https://github.com/JacobTews/preprocessing_and_eda/blob/main/preprocessing_and_eda.ipynb) for your perusal, fully annotated.
