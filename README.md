# sparkify-customer-churn-predict
This Repo contains artifacts related to Udacity's Sparkify Capstone project to predict Customer Churn.

## Project Structure
------
1. [Project Overview](#ProjectOverview)
2. [Key Steps](#Keysteps)
3. [Metrics](#Metrics)
4. [Installation](#Installation)
5. [Files](#Files)
6. [Results and Report](#Results&Report)
7. [References](#References)

------
## 1. Project Overview <a name="ProjectOverview"></a>
Churn also known as attrition or customer churn is the rate at which customers stop doing business with an entity or Organisation.Churn Prediction is a popular problem faced by many businesses. Predicting churn and predicting it well aids businesses with customer retention. As part of this project by predicting which customers are likely to cancel a subscription to its service we are going to help Sparkify a fictional digital music service provider.

In this project, We build an end-to-end machine learning model to predict churn customer based on a sample dataset of Sparkify users data and the Apache Spark Machine Learning libraries.
The model is capable of predict which users is likely to churn the music application service.

## 2. Key Steps <a name="Keysteps"></a>
The goal of this project is to create an end-to-end prediction model of churn users of the Sparkify music application; the tasks involved are the following:
1. Preprocessing (load, clean, and transform) the raw dataset in json format with PySpark
2. Perform Exploratory data analysis and thoroughly analyze the data to come up with the best set of features that can be used to train a predictive model
3. Train and measure models that can predict if a user is is lilely to churn or not by using Apache Spark Machine Learning libraries.
4. Select the best models and improve the models to get higher results
5. Present the results in a report in Medium blog post([this post](https://lgreddy-sbn.medium.com/predicting-churn-using-spark-machine-learning-library-a9b9a1070b0a)) of the end-to-end process to build an ML model in Apache Spark Machine Learning.

## 3. Metrics
1. **F-1 score** (also F-score or F-measure) is a measure of a test's accuracy. It considers both the precision p and recall r of the test to compute the score. This traditional F-measure or balanced F-score is the harmonic mean of precision and recall. F-1 = 2 x (precision x recall) / (precision + recall)

2. **Accuracy** is a common metric for binary classifiers; it takes into account both true positives and true negatives with equal weight: accuracy = (true_positive + true_negatives)/dataset_size.

It is worth mentioning that the dataset provided to us is unbalanced and we mainly rely on F1-Score to measure model's performance.

## 4. Installation <a name="Installation"></a>
The project is run in Apache Spark environment. Refer to [Apache Spark](https://spark.apache.org) to set up an environment for Spark.
+ PySpark - Spark Version 2.4.3
+ Spark MLlib
+ seaborn
+ Pandas
+ matplotlib
+ numpy

## 5. Files <a name="Files"></a>
<pre>
- datasources
|- sample_sparkify_event_data.json
- notebooks
|- Sparkify.ipynb
|- Sparkify.html
- README.md
</pre>

## 6. Results and Report <a name="Results&Report"></a>
The final churn prediction model gets the F-1 score of 75% and Accuracy of 76%.
The report of this project is presented in this blog post [Churn Prediction with Apache Spark Machine Learning](https://lgreddy-sbn.medium.com/predicting-churn-using-spark-machine-learning-library-a9b9a1070b0a).

## 7. References <a name="References"></a>
1. [PySpark](http://spark.apache.org/docs/latest/api/python/)
2. Datasets provided by [Udacity](https://www.udacity.com)
3. [Apache Spark Machine Learning library](https://spark.apache.org/mllib/)
4. [Customer churn using ML](https://www.kdnuggets.com/2019/05/churn-prediction-machine-learning.html)
