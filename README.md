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

NumPy, Pandas, Matplotlib, Json, Plotly, Nltk, Flask, Sklearn, Sqlalchemy, Sys,Re, Pickle

## Project Motivation<a name="motivation"></a>

For this project we have data set containing real messages that were sent during disaster events. We have created a machine learning pipeline to categorize these events so that the messages can be flagged to an appropriate disaster relief agency. The project also includes a web app where an emergency worker can input a new message and get classification results in several categories. The web app has display visualizations of the data.

![file1](https://github.com/Subham-R/Disaster_Responses_Pipelines/blob/master/01%20Overview.PNG)

![file2](https://github.com/Subham-R/Disaster_Responses_Pipelines/blob/master/02%20Distribution%20of%20message%20categories.png)

![file3](https://github.com/Subham-R/Disaster_Responses_Pipelines/blob/master/03%20Top%2010%20tokens.png)

![file4](https://github.com/Subham-R/Disaster_Responses_Pipelines/blob/master/04%20Classify%20Message.PNG)




## File Descriptions <a name="files"></a>

Python core for creating the Plotly charts used in the web app.

ETL Pipeline Preparation.ipynb: This code present in Jupyter notebook was used in the development of process_data.py. 

process_data.py automates ETL Pipeline Preparation.

ML Pipeline Preparation.ipynb: The code and analysis contained in this Jupyter notebook was used in the development of train_classifier.py. In particular, it contains the analysis used to tune the ML model and determine which model to use. 

train_classifier.py automates the ML Pipeline Preparation.

disaster_messages.csv, disaster_categories.csv contain sample messages (real messages that were sent during disaster events) and categories datasets in csv format.

templates folder: This folder contains all of the files necessary to run and render the web app.
custom_transformer.py contains custom functions that were used in ML Pipeline Preparation.ipynb so to find best way of model tuning.

## Run <a name="Run"></a>
Folowing three main files are required for the project:

data/process_data.py
Python code for loading, cleaning, and saving data to a SQL database.

models/train_classifier.py
Python code to classifies text messages into categories.

app/run.py
Python core for creating the Plotly charts used in the web app.

To run ETL pipeline that cleans data and stores in database python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db

To run ML pipeline that trains classifier and saves python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl

Run the following command in the app's directory to run your web app. python run.py
Go to http://0.0.0.0:3001/

## Results<a name="results"></a>

The main findings of the code can be found at the post available [here](https://medium.com/@subham.ronghe/how-does-the-home-stays-listings-are-priced-by-the-airbnb-f5d3eec3701d).

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Must give credit AirBnB and Kaggle for the data and udacity for the structure/template/layout.  You can find the Licensing for the data and other descriptive information at the Kaggle link available [here](https://www.kaggle.com/airbnb/seatle/data).  Otherwise, feel free to use the code here as you would like! 

