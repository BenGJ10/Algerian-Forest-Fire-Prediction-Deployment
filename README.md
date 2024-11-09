# Algerian Forest Fire Prediction Deployment

This repository contains a machine learning project for predicting forest fire occurrences in Algeria based on climatic data. The project uses the Algerian Forest Fire dataset, deploying a Ridge Lasso regression model to predict fire likelihood. The deployment is done through a Flask web application, designed for use with AWS Beanstalk.

## About the Dataset

The dataset includes 244 instances representing data from two regions in Algeria:

- **Bejaia Region**: Located in the northeast of Algeria
- **Sidi Bel-abbes Region**: Located in the northwest of Algeria

The data spans the period from **June 2012 to September 2012** and includes 11 attributes along with a target attribute (class). The dataset is classified into two categories:
- **Fire**: 138 instances
- **Not Fire**: 106 instances

### Attributes

The dataset includes attributes such as temperature, humidity, wind speed, and other climatic and environmental factors, which are used to determine the likelihood of a forest fire.

## Project Structure

The repository is organized as follows:

- `Datasets`: Contains the Algerian Forest Fire dataset.
- `Models`: Contains trained Ridge Lasso regression models.
- `Notebooks`: Contains Jupyter notebooks for data exploration and model training.
- `Templates`: Contains HTML templates for the Flask app.
- `static`: Contains static files, such as CSS, for the web interface.
- `application.py`: The main Flask application file.
- `requirements.txt`: Lists the Python dependencies for the project.

## Model Details

This project uses Ridge and Lasso regression models, which are types of linear regression models with regularization. These models were selected to handle multicollinearity and improve prediction accuracy by reducing overfitting.

### Prerequisites

Make sure you have Python installed. To install the required packages, use:

1. Clone the repository
2. pip install -r requirements.txt
3. To run the flask server: python application.py
4. Open your browser and navigate to http://127.0.0.1:5000 or http://127.0.0.1:5001

## Acknowledgments
- Dataset from UCI Machine Learning Repository: Algerian Forest Fire Dataset.
- Project inspired by Krish Naik's Complete ML - NLP - MLOps Bootcamp.
