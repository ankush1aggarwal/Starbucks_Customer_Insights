# Starbucks_Customer_Insights

## Using Starbucks app data to predict successful offers

This repository has all the code and report done as part of Udacity Machine Learning Engineer with AWS Nanodegree Capstone project.

## 1. Installations
This project was written in Python, using Jupyter Notebook Instance on Amazon SageMaker. The relevant Python packages for this project are as follows:

pandas

numpy

math

sklearn.model_selection (train_test_split module)

sklearn.preprocessing (StandardScaler)

from sklearn.tree (DecisionTreeClassifier)

sklearn.ensemble (RandomForestClassifier)

sklearn.metrics (classification_report)

time

matplotlib

## 2. Project Motivation
This project is the Capstone project of my Machine Learning Engineer with AWS Nanodegree with Udacity. For the challenge, Udacity provided simulated data that mimics customer behavior on the Starbucks rewards mobile app.

In this project, I use the data to answer 2 main questions:

a. What are the main characteristics of an succesful offer?
b. Based on the characteristics identified above, Predict if a particular user would take up an offer?

To answer the above 2 questions, I created 3 models for the data on the 3 offer types provided. The three offers are: Buy One Get One Free (BOGO), Discount (discount with purchase), and Informational (provides information about products).

As a brief summary of my findings:

For a), the feature importance given by all 3 models were that the tenure of a member is the biggest predictor of the success of an offer. Further, the top 4 variables were the same - membership tenure, income, age and day of offer. However, income and age switched orders depending on offer type.

For b), my decision to use 3 separate models to predict the success of each offer type ended up with good accuracy for the 2 of the models (81.58% for BOGO and 86.59% for discount), while slightly less accurate performance for another informational offers (73.7%). However, I would regard this as acceptable in a business setting, as for informational offers, there is no cost involved to inform users of a product. 

## 3. File Descriptions
This repo contains 4 files. The notebook of my project is called 'Starbucks_Capstone_notebook.ipynb'. The data used in the project is in the files portfolio.json, profile.json and transcript.json.

## 4. Licensing, Authors, Acknowledgements, etc.
Data for coding project was provided by Udacity.
