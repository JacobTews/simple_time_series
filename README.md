# Sample project: Time-series analysis

### "HR has requested some help with a project," my team lead, Jordan, explained

"They have data from a survey given to a bunch of managers, and they'd like you to go through it to find:
* the average salary for a software engineer for each currency,
* the average salary for a software engineer for each currency _grouped by age_, and
* a comparison of the four currencies which are most common in the data.

"And just a heads up: the data is a bit messy, since there are some free-response text fields in the survey, so it will need some cleaning. You'll also need to grab currency conversions to compare the salaries.

"They need the information by the end of the day."

"I'm on it!" I replied, and headed back to my desk to get started...

## 🎯 Goals
* Explore the dataset, handling missing entries.
* Convert all salaries for software developers and engineers to USD.
* Determine the average software engineer salary for each currency and the average salary for each currency based on age.
* Visualize a comparison by plotting the salaries based on age for the top 4 currencies in the merged dataset

## 🏗 Dependencies
* Python 3.9.7
* matplotlib.pyplot
* numpy
* pandas
* re
* seaborn

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
