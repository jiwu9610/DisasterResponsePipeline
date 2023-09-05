# Disaster Response Pipeline Project

This project is part of the Data Scientist Nanodegree program by Udacity. The goal of this project is to build a machine learning model that can classify disaster response messages into different categories. The project includes an ETL pipeline, a machine learning pipeline, and a web app to visualize the results.

## Table of Contents
- [Installation](#installation)
- [Project Motivation](#project-motivation)
- [File Descriptions](#file-descriptions)
- [Instructions](#instructions)
- [Results](#results)
- [Licensing, Authors, and Acknowledgements](#licensing-authors-and-acknowledgements)

## Installation
To run this project, you need to have Python 3.x installed. Clone this repository and install the required libraries using the following command:
pip install -r requirements.txt


## Project Motivation
In the event of a disaster, it is crucial to quickly identify relevant messages and classify them into different categories to provide appropriate aid and support. This project aims to build a machine learning model that can automate this process and help responders prioritize their actions.

## File Descriptions
- `data` folder: Contains the raw data and the ETL pipeline script.
- `models` folder: Contains the machine learning pipeline script and the trained model.
- `app` folder: Contains the web app files.

## Instructions
1. Run the ETL pipeline to clean the data and store it in a SQLite database. Use the following command:
python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db


2. Run the machine learning pipeline to train the classifier and save the model. Use the following command:
python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl


3. Start the web app to visualize the results. Use the following command:
cd app python run.py


4. Access the web app by visiting `http://localhost:3001` in your web browser.

## Results
The machine learning model is trained on the provided dataset and can classify disaster response messages into different categories. The web app provides a user-friendly interface to input messages and view the classification results.

## Licensing, Authors, and Acknowledgements
This project is licensed under the MIT License. The dataset used in this project is provided by Figure Eight and the initial code template is provided by Udacity.
