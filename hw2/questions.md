# 2. Exploratory Data Analysis and Data Cleaning
## 2.1. Why do we explore / clean data?
1. One of these is *not* a _Why?_ reason for EDA?
* Understand the shape of the data
* Learn which features might be useful
* Start thinking about appropriate model architecture <--
* Inform the cleaning that will follow
2. One of these is *not* a _Why?_ reason for Data Cleaning?
* Perform feature selection <--
* Shape data so model can pick up on signal
* Remove irrelevant data
* Adjust features to be acceptable for model
## 2.2. Exploring continuous features
1. What's an aggregate operation we can use to understand different variables relationship with our target?
* Merge on
* Group by <--
* Select
* Filter out
2. Which one of these stats is not returned by the `pd.DataFrame.describe()` method?
* Min
* Mean
* Standard deviation
* Skewness <--
## 2.3 Plotting continuous features
1. In seaborn (aliased in video as `sns`) which function shows us a histogram?
* `sns.hist()`
* `sns.distplot()`
* `sns.plot()`
* `sns.h()`
2. Ultimately, what did plotting allow us to do?
* Understand why we should drop some features
* Where the nulls where
* That we could create an aggregated feature <--
* Nothing
## 2.4 Continuous data cleaning
1. Which one of these is *not* a good idea to use as a proxy for a `null` Age variable?
* The sample mean
* The median
* Zero <--
2. What's the pandas function that allows you to impute `null` values?
* `replace`
* `remove_nulls`
* `fillna` <--
* `findandreplace`
## 2.5 Exploring categorical features
1. What's the statistic we want to understand with `group_by`
* Correlations with other features
* Ratios to the total population (class prior) <--
* Prior Probability
* Which features to drop
2. What's a way to represent meaningful missing categories?
* An indicator variable
* Just drop them
* Replace them with the most popular class
* Randomize them
## 2.6 Plotting categorical features
1. What seaborn plot gets used here?
* `sns.plot()`
* `sns.barchart()`
* `sns.barplot()`
* `sns.catplot` <--
2. If we want to understand whole ratios for different groups in a `pivot_table` what do we pass to `aggfunc`?
* `'count'` <--
* `'sum'`
* `'mean'`
* `'max'`
## 2.7 Categorical data cleaning
1. What can we do with multi-label text fields?
* Drop them
* One-hot encoding <--
* Turn them into byte representations to vectorize them
* Randomize them
2. What numpy `np` function gets used to create a boolean mask?
* `np.if`
* `np.where` <--
* `np.get`
* `np.show`
