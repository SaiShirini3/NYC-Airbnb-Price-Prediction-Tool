# NYC Airbnb Analysis

This repository contains the code and documentation for the project "NYC Airbnb Analysis," aimed at predicting Airbnb listing prices based on various features using machine learning techniques and deploying the model through a Flask web application.

## Table of Contents

- [Introduction](#introduction)
- [Problem Statement](#problem-statement)
- [Project Approach](#project-approach)
- [Data Source](#data-source)
- [Project Execution](#project-execution)
- [Results](#results)
- [Conclusion](#conclusion)
- [Future Enhancements](#future-enhancements)
- [Files](#files)
- [Usage](#usage)
- [Contributors](#contributors)
- [License](#license)

## Introduction

The advent of online platforms like Airbnb has revolutionized the hospitality industry. This project aims to leverage data analysis and machine learning techniques to predict the prices of Airbnb listings based on relevant features. The findings can provide valuable insights for both hosts and guests, optimizing pricing strategies and enhancing user experience.

## Problem Statement

The project focuses on exploring the relationship between various Airbnb listing attributes such as location, room type, minimum nights, availability, and their influence on listing prices. The goal is to uncover significant factors influencing pricing variations across different neighborhoods and property types.

## Project Approach

### Techniques Used
- **Data Cleaning and Preprocessing**: Ensuring data quality by handling missing values and standardizing data.
- **Exploratory Data Analysis (EDA)**: Understanding data distribution and correlations between features.
- **Predictive Modeling**: Implementing various machine learning models to predict listing prices.
- **Model Deployment**: Integrating the best-performing model into a Flask web application.

### Machine Learning Models Used
1. Linear Regression
2. Support Vector Machine (SVM)
3. K-Means Clustering
4. Polynomial Regression
5. Decision Tree
6. Random Forest
7. Ridge Regression

## Data Source

The dataset used for this project is the NYC Airbnb Open Data from Kaggle. It contains 48,895 data points with 16 features, including attributes like neighborhood, room type, price, and availability.

- [Dataset Link](https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data)

## Project Execution

### Data Loading and Preprocessing
- Loaded the dataset and performed data cleaning, including handling missing values and standardizing textual data.
- Converted relevant columns to appropriate data types for analysis and modeling.

### Modeling and Evaluation
- Trained and evaluated several machine learning models to predict Airbnb listing prices.
- Selected the Random Forest model for its superior performance in terms of R-squared and Mean Squared Error (MSE).

### Model Deployment
- Developed a Flask web application to deploy the Random Forest model.
- Created a user-friendly interface using HTML, CSS, and Bootstrap for users to input listing features and receive price predictions.

## Results

- **Random Forest Model**: Achieved the best performance with an R-squared score of 0.599 and MSE of 0.0363, indicating that approximately 60% of the variance in Airbnb prices can be explained by the model.
- **Visualization**: Developed interactive visualizations to help users explore the relationship between different features and listing prices.

## Conclusion

The project successfully demonstrated the application of machine learning techniques to predict Airbnb listing prices. The deployment of the model through a web application provides a practical tool for users to make data-driven decisions regarding Airbnb pricing.

## Future Enhancements

- Integrate real-time market data to improve the accuracy of price predictions.
- Incorporate user reviews and ratings to provide a more comprehensive pricing model.
- Expand the model to include external economic factors and their impact on pricing dynamics.

## Files

- `app.py`: Flask application code.
- `code.ipynb`: Jupyter notebook with data analysis and modeling.
- `wdbc.data`: Data file used in the project.
- `wdbc.names`: Column names for the dataset.
- `biplot.png`: Biplot of PCA results.
- `scree.png`: Scree plot for PCA results.
- `report1.pdf`: Phase 1 project report.
- `report2.pdf`: Phase 2 project report.
- `report3.pdf`: Phase 3 project report.
- `Project Final Report.pdf`: Detailed project report.
- `Breast Cancer Awareness.pptx`: Presentation slides.
- `Demo.mp4`: Video demonstration of the project.

## Usage

### Initial Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/nyc-airbnb-analysis.git
2. Navigate to the project directory:
   ```bash
   cd nyc-airbnb-analysis
3. Install the required packages:
     ```bash
   pip install -r requirements.txt

## Running the Flask Application

1. Ensure that all HTML files are placed in the designated templates folder within the Flask application directory.
2. Load the Random Forest model, ensuring the pickle file is correctly placed in a known directory.
3. Start the Flask application:
    ```bash
   python app.py
5. Open a web browser and go to http://localhost:5000 to access the application.

## Using the Web Application

1. Navigate to the main page (home route /) to find the prediction and visualization tools.
2. For predictions, fill out the form with Airbnb listing details such as neighborhood group, room type, minimum nights, and other relevant features, then submit the form.
3. The Flask backend processes the request, and the predicted price is displayed on the page.
4. For visualizations, select the desired features and graph type, then generate the visualization to explore data patterns and correlations.
   



 



   



