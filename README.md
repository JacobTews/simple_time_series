# Sample project: Time-series analysis

### Today I got a note from Tim Seres, the store manager for the downtown branch.

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
* __The model can be used for staffing decisions ~6 weeks into the future.__
* __When spikes in sales volume are predicted, ~40% should be added to that predicted number when scheduling sales reps.__
* The general contour of the predictions closely matches the actual sales, suggesting that when a spike is predicted, more sales reps should be scheduled, even if the actual size of the spike isn't perfectly accurate.

![sales predictions vs. actual sales](https://github.com/JacobTews/simple_time_series/blob/e0d999eae0e7575f11633bdd9c1b78f3f7a75d03/viz/best_model_preds.png?raw=true)

* The model tends to underestimate sales spikes by ~40%, so if one rep can handle ~ \\$1000 in daily sales, and a spike of $3000 is predicted, 4 reps should be scheduled.
* Hybrid model predictive accuracy declines significantly 100+ days in the future, so long-term hiring decisions are better informed by the simple linear model.

![linear model shows trend](https://github.com/JacobTews/simple_time_series/blob/c450fc6369139b64110b64d498ff52d766b57b84/viz/linear_regression.png)

* For further study:

&emsp;&emsp;&emsp;Why is there a 50-day lagging trend in sales?

&emsp;&emsp;&emsp;Can I get the same predictive power with only the lagging data, to make sure there's no information leakage in the model?

## 🛠 Want to dig into my code?
Here's the [notebook](https://github.com/JacobTews/simple_time_series/blob/6accaec676f46096145079196a7b48afc831506b/time_series_analysis.ipynb) for your perusal, fully annotated.
