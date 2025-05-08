# Formula 1 Race Prediction Model

This repository contains a Jupyter Notebook (`ML_project_3.ipynb`) and a project report (`report.pdf`) for scraping, preprocessing, modeling, and visualizing Formula 1 race result predictions.

## Table of Contents
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Data Collection](#data-collection)
- [Data Preprocessing](#data-preprocessing)
- [Model Training](#model-training)
- [Evaluation](#evaluation)
- [Report](#report)
- [Dependencies](#dependencies)

## Project Structure
├── ML_project_3.ipynb # Main Jupyter notebook with end-to-end pipeline
├── report.pdf # Detailed project report
└── README.md # This file


## Installation

1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd <repository_folder>

   python3 -m venv venv
   source venv/bin/activate   # macOS/Linux
   venv\Scripts\activate      # Windows

2.pip install pandas numpy matplotlib seaborn scikit-learn xgboost tensorflow requests

## Usage
Open the notebook:

jupyter notebook ML_project_3.ipynb

Run cells in order to:

Scrape data from the Ergast API for specified seasons

Preprocess and clean the dataset

Engineer features and split into training and test sets

Train Random Forest, XGBoost, and Neural Network models

Evaluate and visualize model performance

Adjust parameters (e.g., seasons, model hyperparameters) at the top of each section as needed.



## Data Collection

Uses the Ergast Developer API to fetch historical race data, qualifying results, driver standings, and constructor standings.
Implements robust error handling and logging for API requests.

## Data Preprocessing

Cleans raw data by handling missing values, converting types, and merging tables.
Engineers features such as qualifying position, driver experience, and constructor performance metrics.

## Model Training

Builds a scikit-learn pipeline for each model:
Random Forest Regressor
XGBoost Regressor
Keras Neural Network
Includes grid search for hyperparameter tuning.

## Evaluation

Compares models using RMSE and MAE on the test set.
Visualizes predictions vs actual positions.

## Report

Detailed methodology, results, and discussion are available in report.pdf.

## Dependencies

Python 3.7+
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
tensorflow
requests

