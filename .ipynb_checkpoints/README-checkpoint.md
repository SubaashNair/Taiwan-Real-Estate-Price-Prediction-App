# Taiwan Real Estate Price Prediction App

![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
![scikit-learn](https://img.shields.io/badge/sklearn-1.1.1-orange.svg)
![pandas](https://img.shields.io/badge/pandas-1.4.3-blue.svg)
![seaborn](https://img.shields.io/badge/seaborn-0.11.2-blue.svg)
![Gradio](https://img.shields.io/badge/gradio-3.1.1-green.svg)

## Objective
The primary objective of this project is to develop a machine learning model that predicts the price per square meter of real estate in Taiwan. The model is deployed as an interactive web application using Gradio, allowing users to input property features and receive instant price predictions.

## Dataset
The dataset used in this project is the `taiwan_real_estate2.csv`, which contains real estate data from Taiwan. The dataset includes the following features:
- `dist_to_mrt_m`: Distance to the nearest MRT station in meters.
- `n_convenience`: Number of convenience stores within walking distance.
- `house_age_years`: The age of the house in years.
- `price_twd_msq`: Price of the real estate per square meter (target variable).

## Machine Learning Model
Several regression models were evaluated for this task, including:
- Linear Regression
- Ridge Regression
- Lasso Regression
- Elastic Net Regression
- Decision Tree Regression
- Random Forest Regression
- Gradient Boosting Regression

The Random Forest Regression model was selected based on its balance between performance and generalization, as evidenced by evaluation metrics on both training and test datasets.

## Outcome
The final Random Forest model demonstrates the ability to predict real estate prices with reasonable accuracy. The model was deployed via a Gradio app, providing a user-friendly interface for interactive predictions.

## App Interface

Below is a screenshot of the web application interface:

![App Screenshot](images/app.png)
![App Screenshot](images/app2.png)

This image shows the Gradio web interface for the real estate price prediction model, demonstrating the input fields and prediction output.


## How to Use
To use the prediction app:
1. Clone the repository to your local machine.
2. Install the requirements using `pip install -r requirements.txt`.
3. Run the Gradio app script.
4. Input the features of the property in the web interface.
5. View the predicted price per square meter.

---
