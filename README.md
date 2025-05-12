# Fraud Detection System

## Overview

This notebook implements a fraud detection system using machine learning. It analyzes a dataset (likely containing financial transaction data) to identify fraudulent activities. The system takes transaction features as input and predicts whether a transaction is fraudulent or not.

## Features

* **Data Loading and Exploration**:  Loads the dataset using pandas and performs initial exploration.
* **Data Preprocessing**:
    * Handles missing values.
    * Removes duplicate entries.
    * Visualizes the class distribution of the target variable ('Class').
* **Data Scaling**: Scales the features using `StandardScaler` to ensure optimal performance for machine learning models.
* **Model Training and Evaluation**:
    * Splits the data into training and testing sets.
    * Trains a Logistic Regression model.
    * Evaluates the model's performance using accuracy, a classification report, and a confusion matrix.
* **User Interface**:
    * Creates a user interface using Gradio.
    * Allows users to input transaction features.
    * Predicts whether the transaction is fraudulent or not.

## Technical Details

* **Programming Language**: Python
* **Libraries**:
    * pandas
    * numpy
    * matplotlib.pyplot
    * seaborn
    * scikit-learn
    * Gradio

## How to Use

1.  **Prepare the Data**: Ensure the data is in a CSV file named `creditcard.csv` and placed in the same directory as the notebook.
2.  **Run the Notebook**: Open and run the notebook in a Jupyter environment.
3.  **Interact with the UI**: Once the notebook has been executed, a Gradio interface will appear, allowing you to enter transaction details and get a fraud prediction.

## Input Features

The user interface requires the following features as input:

* Time
* V1 - V28
* Amount

## Output

The system will output one of the following:

* Fraud
* Not Fraud
