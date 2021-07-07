# Predicting User Churn with Apache Spark
![Cover](sparkify.png)

## Medium:
[How to predict user churn with PySpark on Big Data](https://tioans.medium.com/how-to-predict-user-churn-with-pyspark-on-big-data-f5922865d72b)

## About

The goal of this project is to create a system capable of predicting the rate of user churn for "Sparkify", a (fictional) popular service for music streaming, similar to Spotify or Apple Music. Predicting churn rates is a challenging and common problem for data scientists working in a customer-facing business. In addition, the ability to manipulate large datasets with Spark is highly regarded in industry. 

The dataset contains user logs with information about about users and their behavior, such as unique IDs, timestamps, session info, subscription type and user actions. Based on this data, a number of distributed ML models were developed and the best performing was selected as default. While the current models were trained on a relatively small (128 MB) dataset, the system can scale to large datsets (more than 12 GB) on cloud services, such as Elastic Map-Reduce (EMR), on AWS. The datasets originate from Udacity.



Project breakdown:
1. **Data Cleaning:** load and clean the data, checking for invalid or missing entries (i.e. no user IDs).
2. **Exploratory Data Analysis:** defining churn, comparing the behavior of users with churned vs those who didn't.
3. **Feature Engineering:** building features after exploring the data for training models.
4. **Modelling:** splitting the dataset into train/val/test sets, comparing several ML methods and evaluation the performance (accuracy and F1 scores).

Model performance:
* Best model: Gradient-boosted tree (GBT); Accuracy: 0.8059 ; F1: 0.7950

## Dependencies

* Python 3.8
* PySpark
* Pandas
* Matplotlib
* Seaborn

## File breakdown 

* 'Sparkify.html' : HTML version of the Jupyter Notebook.
* 'Sparkify.ipynb:' : Main project file, Jupyter Notebook used to develop the system.

## Instructions:
1. Clone the repository.
2. Install dependencies.
3. Run notebook.

## Future work
Based on the model results, the next step would be to deploy to system to AWS's EMR and get results from the large dataset (12 GB). In addition, a web application could be deployed to illustrate results in an interactive way. 

## Acknowledgments
Thanks to the Udacity team for the good guidance and a well-made course. In addition, I'd like to thank Spark team for providing quality documentation.
