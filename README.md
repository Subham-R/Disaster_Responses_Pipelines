# Disaster Responses Pipelines


### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Run](#Run)
5. [Results](#results)
6. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

This project requires Python 3.x and the following Python libraries installed:

NumPy, Pandas, Matplotlib, Json, Plotly, Nltk, Flask, Sklearn, Sqlalchemy, Sys, Re, Pickle

## Project Motivation<a name="motivation"></a>

For this project we have data set containing real messages that were sent during disaster events. We have created a machine learning pipeline to categorize these events so that the messages can be flagged to an appropriate disaster relief agency. The project also includes a web app where an emergency worker can input a new message and get classification results in several categories. The web app has following display visualizations:

![file1](https://github.com/Subham-R/Disaster_Responses_Pipelines/blob/master/01%20Overview.PNG)

![file2](https://github.com/Subham-R/Disaster_Responses_Pipelines/blob/master/02%20Distribution%20of%20message%20categories.png)

![file3](https://github.com/Subham-R/Disaster_Responses_Pipelines/blob/master/03%20Top%2010%20tokens.png)

![file4](https://github.com/Subham-R/Disaster_Responses_Pipelines/blob/master/04%20Classify%20Message.PNG)

## File Descriptions <a name="files"></a>

ETL Pipeline Preparation.ipynb: This code present in Jupyter notebook was used in the development of process_data.py. 
process_data.py: automates ETL Pipeline Preparation.

ML Pipeline Preparation.ipynb: This code was used to tune the ML model and  use in the development of train_classifier.py. 
train_classifier.py automates the ML Pipeline Preparation.

disaster_messages.csv has sample messages
disaster_categories.csv has categories datasets 

templates folder: This folder has files necessary to run web app.

## Run <a name="Run"></a>
Folowing three main files are required for the project:

data/process_data.py
Python code for loading, cleaning, and saving data to a SQL database.

models/train_classifier.py
Python code to classifies text messages into categories.

app/run.py
Python core for creating the Plotly charts used in the web app.

## Results<a name="results"></a>

Go to http://0.0.0.0:3001/ (https://view6914b2f4-3001.udacity-student-workspaces.com/)

Dataset has distribution of message genres: news (highest), direct , social(lowest); distribution of categories and top 10 tokens

It can alaso take a new message  as input and get classification results in several categories

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Must give credit to figure eight for the data and udacity for the structure/template/layout/app. This app was build as part of udacity course.
