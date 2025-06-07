# price-nest
# Real Estate Price Prediction - Data Science Project

## Project Overview

This project demonstrates the end-to-end process of building and deploying a machine learning model to predict real estate prices.

### 1. Machine Learning Model
We build a robust regression model using Scikit-Learn’s **Linear Regression** algorithm on a real estate dataset. The process includes key stages of the machine learning pipeline:

- Loading and cleaning data  
- Detecting and removing outliers  
- Feature engineering to improve model performance  
- Dimensionality reduction techniques  
- Hyperparameter tuning with GridSearchCV  
- Model validation using K-Fold Cross Validation  

### 2. Model Persistence with Pickle
After training, the model is serialized using Python’s `pickle` module — saving the trained model to disk to enable reuse without retraining. This serialized model file is loaded by the web server for prediction.

### 3. Flask Web API
A lightweight Python Flask server is created to serve the trained model via HTTP API endpoints. The server:

- Loads the saved model at startup  
- Receives prediction requests with home details in JSON format (e.g., square footage, bedrooms)  
- Returns predicted house prices as JSON responses  

This demonstrates how machine learning models can be deployed as REST APIs for real-time predictions.

### 4. Frontend Web Interface
A responsive website built with HTML, CSS, and JavaScript that interacts with the Flask backend:

- Users input home features via a simple form  
- The frontend sends data to the Flask API  
- The predicted price is displayed dynamically on the page  

---

## Concepts and Tools Covered

- **Machine Learning:** Model training, validation, hyperparameter tuning, and evaluation  
- **Data Science:** Data cleaning, outlier detection, feature engineering, dimensionality reduction  
- **Model Serialization:** Using Python’s pickle module for saving and loading models  
- **Web Development:**  
  - Backend: Flask API development and handling HTTP POST requests  
  - Frontend: Interactive UI with HTML, CSS, JavaScript  
- **Data Visualization:** Using Matplotlib to analyze and visualize dataset features  
- **Development Environments:** Jupyter Notebook, Visual Studio Code, PyCharm  

---

## Technologies Used

- Python (for data processing and backend)  
- Numpy and Pandas (data manipulation)  
- Matplotlib (data visualization)  
- Scikit-learn (modeling)  
- Pickle (model serialization)  
- Flask (API server)  
- HTML, CSS, JavaScript (frontend UI)  

---

## How to Use

1. Train and save the model by running the training script  
2. Start the Flask server which loads the saved model  
3. Open the web app and enter home features to get price predictions  

---

## Summary

This project provides a hands-on introduction to the end-to-end process of building and deploying machine learning models as web applications, combining data science best practices with software engineering fundamentals.


