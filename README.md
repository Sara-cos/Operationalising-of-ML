# Opeartionalising of Machine Learning
## Overview
In this project a model is trained using Automated Machine Learning. Then it is operationalised using Microsoft Azure Machine Learning. 

The dataset used here is a information of Portuguese Bank Marketing. The informations is based on phone calls , age, type of job, marital, education, has credit in defualt, housing, loan, type of contact , last contact, day of the week of the contact, duration in seconds, campaigns, and other variables. We want to predict if the client has subscribed a term deposit.
The csv file consist of 32950 row and 21 columns. The csv file(https://automlsamplenotebookdata.blob.core.windows.net/automl-sample-notebook-data/bankmarketing_train.csv). Here the loan column is the targeted column.

The steps involved:-
1. An AutoML model is trained using the Bank Marketing dataset.
2. Deployed the best model to an ACI (Azure Container Instance) using Azure ML Studio.
3. We enable the Application Insights feature and review the generated logs using the logs.py script.
4. We publish the deployed model API swagger documentation by running a docker container in our localhost. For which download the endpoint swagger.json file from Azure ML.
5. We consume the scoring API to clasify new instances by running the endpoint.py script in our localhost. We must get the scoring_uri and key for the deployed model endpoint and update the script.
6. Used Apachebenchmark for testing the model.

### Pipeline Automation
