
### Sparkify Project

## Installation <a name="installation"></a>

* Pyspark
* Pandas
* Numpy
* Matplotlib

## Project Overview<a name="overview"></a>

For this project, We are studying the event log data of users of Sparkify, a music streaming provider like Spotify. In the project, we are trying to utilize the data to predict the "churn" rate, i.e., when users downgrade their servivce levels.

## Problem Statement<a name="statement"></a>

We are trying to generate user statistics from the user event log data and use a machine learning model to predict the churning users.

## Metrics<a name="metrics"></a>

The accuracy metric is used to measure the performance of models.

## Exploratory Data Analysis<a name="eda"></a>

After loading the data set, we perform exploratory data analysis to better understand the data.

## Data Preprocessing<a name="dp"></a>

We performed data preprocessing to get rid of invalid data, and generate the churn label.

## Feature Engineering <a name="fe"></a>

After loading the data set, we conducted a series of operations to extract features set including average song listened per session for each user.

## Modelling<a name="modeling"></a>

We built 3 models: logistic regression, decision tree classifier and random forest with the generated features and train the data on the training set while use the test set to measure the final performance of each model.

Among the 3 models: logistic regression, decision tree classifier and random forest, they all over achieved accuray s with accuracy around 70%. The Logistic Regression model has the highest accuracy at around 70.27%.

We used 3 fold cross validation to fine-tune the models, on the "regParam" and "elasticNetParam" of the Logistic Regression, the overall accuracy improved a bit to around 70.37% on the testing set.

## Results<a name="results"></a>

After the model selection and hyperparameter tuning, the logistic regression model achieved around 70.37%.

The main findings of the code can be found at the post available [here](https://orientsun6.medium.com/predicting-user-churn-with-pyspark-5f5fb0fdb835).

## File Descriptions <a name="files"></a>

Sparkify.ipynb: containing the analysis.  Markdown cells were used to assist in walking through the thought process for individual steps.

mini_sparkify_event_data.json.zip: data zip file.