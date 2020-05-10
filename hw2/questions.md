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
# 3 Measuring Success
## 3.1 Why split data?
1. What ultimate goal drives our desire to split our data?
* Trying to build a generalizable model <--
* Testing which data to train on
* There is no reason
* See how much data we need to train on
2. What are the three datasets we need to create?
* Train, test, question
* Train, copy, split
* Train, test, validation <--
* Validation, deploy, test
## 3.2 Split data
1. What's an appropriate percent for the validation set?
* 90%
* 2%
* 5%
* 20% <--
2. If we want our splits to be reproducible which parameter of `train_test_split` would we explicitly provide?
* `random_state` <--
* `do_over`
* `reproduce_number`
* `state`
## 3.3 What is cross-validation?
1. What is k-fold cross validation?
* Partition dataset into k+1 sets, train on k and test on k+1
* Partition dataset into k sets, train on k-1 and test on k
* Partition dataset into k sets, train on k-2, test on k-1, and validation on k
* Partition dataset into k sets and train on a random number of k-n, test on n  
2. What statistic is used to define the performance in k-fold cross validation?
* Mean <--
* Max
* Floor
* Ceiling
## 3.4 Evaluation framework
1. We want to know the ratio of true positives to all predictions, which stat do we want?
* Recall
* Precision <--
* Sensitivity
* Generalization
2. What does recall give us?
* The ratio of true negatives to false negatives
* The ratio of total negatives to correctly predicted negatives
* The ratio of true positives to total positive class instances <--
* The ratio of true negatives to total negative class instances
# 4 Optimizing a model
## 4.1 Bias / Variance trade-off
1. What is bias in the context of this lesson?
* A shift parameter
* Tendency to consistently learn the wrong thing by not considering all available information <--
* The available signal-to-noise ratio
* Your assumptions about the data
2. What is variance in the context of this lesson?
* The algorithm's sensitivity to changes in the data <--
* The squared distance from the mean
* The available signal-to-noise ratio
* How much you can shift the bias and still get it right
## 4.2 Underfitting
1. Total error is...
* (Bias + Variance) + Noise <--
* (Bias - Variance)
* (Bias + Variance)
* (Bias - Variance) + Noise
2. Underfitting is _always_ result of
* The model not capturing the underlying trend of the data <--
* Not including enough parameters in our model
* Not normalizing our features
* Using the wrong model architecture
## 4.3 Overfitting
1. Overfitting can be caused by...
* Not normalizing our features
* Over-parameterizing our model on small amounts of data <--
* Using all available features
* Normalizing our features
2. What can a decision boundary tell us about overfitting
* If it's not smooth enough we might have overfit <--
* If its too smooth we might have overfit
* It can't tell us anything
* If it's shifted we might have overfit
## 4.4 Optimal trade-off
1. What trade-off are we optimizing for?
* Bias v Variance <--
* Error v Total error
* Accuracy v error
* In-sample v out-of-sample
2. What metric tells us we're doing something right?
* Train accuracy
* Test error <-
* Train error
* Sensitivity
## 4.5 Hyperparameter tuning
1. How do we define a hyperparameter?
* A weight within the model
* An output value
* A model configuration <--
* A bias measure
2. Which one of these is _not_ a hyperparameter for a Decision Tree?
* max_depth
* min_split
* accuracy threshold <--
* split metric (e.g. entropy)
## 4.6 Regularization
1. Regularization defends us against...
* Overfitting <--
* Underfitting
* Over Bias
* Not converging
2. Which one of these is _not_ a regularization technique?
* Ridge regression
* Lasso regression
* Dropout
* Test twice <--
