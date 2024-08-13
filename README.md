# NYC Airbnb Analysis

Welcome to the "NYC Airbnb Analysis" project repository. This project aims to predict Airbnb listing prices using various machine learning techniques, with the model deployed via a Flask web application.

## Table of Contents
1. [Introduction](#introduction)
2. [Problem Statement](#problem-statement)
3. [Project Approach](#project-approach)
   - [Techniques Used](#techniques-used)
   - [Machine Learning Models Used](#machine-learning-models-used)
4. [Data Source](#data-source)
5. [Project Execution](#project-execution)
   - [Data Loading and Preprocessing](#data-loading-and-preprocessing)
   - [Modeling and Evaluation](#modeling-and-evaluation)
   - [Model Deployment](#model-deployment)
6. [Results](#results)
7. [Conclusion](#conclusion)
8. [Future Enhancements](#future-enhancements)
9. [Files](#files)
10. [Usage](#usage)
    - [Initial Setup](#initial-setup)
    - [Running the Flask Application](#running-the-flask-application)
    - [Using the Web Application](#using-the-web-application)

## Introduction
The rise of platforms like Airbnb has significantly transformed the hospitality industry. This project utilizes data analysis and machine learning to predict Airbnb listing prices based on various features. The insights generated can help hosts optimize pricing strategies and enhance the guest experience.

## Problem Statement
This project aims to explore the relationship between various attributes of Airbnb listings, such as location, room type, and availability, to predict listing prices. By identifying significant factors influencing price variations, the project provides actionable insights for both hosts and guests.

## Project Approach

### Techniques Used
1. **Data Cleaning and Preprocessing:** Addressed missing values, standardized data, and converted relevant columns to appropriate data types.
2. **Exploratory Data Analysis (EDA):** Analyzed data distribution and correlations between features to understand underlying patterns.
3. **Predictive Modeling:** Implemented and evaluated several machine learning models to predict listing prices.
4. **Model Deployment:** Deployed the best-performing model using a Flask web application with an intuitive user interface.

### Machine Learning Models Used
- Linear Regression
- Support Vector Machine (SVM)
- K-Means Clustering
- Polynomial Regression
- Decision Tree
- Random Forest
- Ridge Regression

## Data Source
The dataset used is the NYC Airbnb Open Data from Kaggle. It comprises 48,895 entries and 16 features, including neighborhood, room type, price, and availability.

## Project Execution

### Data Loading and Preprocessing
- **Data Loading:** Imported the dataset and performed data cleaning.
- **Preprocessing:** Managed missing values, standardized textual data, and converted columns to suitable data types.

### Modeling and Evaluation
- **Training:** Trained multiple machine learning models on the dataset.
- **Evaluation:** Selected the Random Forest model for its best performance based on R-squared and Mean Squared Error (MSE) metrics.

### Model Deployment
- **Web Application:** Developed a Flask web app to deploy the Random Forest model.
- **User Interface:** Designed a user-friendly interface using HTML, CSS, and Bootstrap, allowing users to input listing features and obtain price predictions.

## Results
- **Model Performance:** The Random Forest model achieved an R-squared score of 0.599 and an MSE of 0.0363, explaining approximately 60% of the variance in Airbnb prices.
- **Visualizations:** Created interactive visualizations to explore the relationships between different features and listing prices.

## Conclusion
The project successfully applied machine learning techniques to predict Airbnb listing prices and provided a practical tool for making data-driven pricing decisions. The deployment of the model as a web application allows users to interact with and benefit from the analysis.

## Future Enhancements
1. **Real-Time Data Integration:** Incorporate real-time market data to improve price prediction accuracy.
2. **User Reviews and Ratings:** Include user reviews and ratings to create a more comprehensive pricing model.
3. **External Factors:** Expand the model to consider external economic factors and their impact on pricing dynamics.

## Files
- **app.py:** Flask application code.
- **code.ipynb:** Jupyter notebook with data analysis and modeling.
- **wdbc.data:** Dataset file used in the project.
- **wdbc.names:** Column names for the dataset.
- **biplot.png:** Biplot of PCA results.
- **scree.png:** Scree plot for PCA results.
- **report1.pdf:** Phase 1 project report.
- **report2.pdf:** Phase 2 project report.
- **report3.pdf:** Phase 3 project report.
- **Project Final Report.pdf:** Detailed project report.
- **Breast Cancer Awareness.pptx:** Presentation slides.
- **Demo.mp4:** Video demonstration of the project.

## Usage

### Initial Setup
1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/nyc-airbnb-analysis.git
2. **Navigate to the project directory:**
     ```bash
   cd nyc-airbnb-analysis
3. **Install the required packages:**
      ```bash
   pip install -r requirements.txt

## Running the Flask Application
1. **Prepare HTML files:** Ensure all HTML files are in the `templates` folder within the Flask application directory.
2. **Load the model:** Ensure the Random Forest model pickle file is correctly placed in a known directory.
3. **Start the Flask application:**
   ```bash
   python app.py
4. **Access the Application:** Open a web browser and go to `http://localhost:5000` to interact with the app.

## Using the Web Application
- **Prediction:** Navigate to the main page, fill out the form with listing details (e.g., neighborhood, room type, minimum nights), and submit to get the predicted price.
- **Visualization:** Use the tools provided to generate visualizations and explore data patterns and correlations.



