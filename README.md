

---

# NYC Airbnb Price Prediction Tool

## Overview
This repository contains a machine learning project aimed at predicting Airbnb listing prices in New York City based on various attributes of the listings. The tool leverages data from thousands of Airbnb listings, incorporating features like neighborhood details, room type, minimum stay requirements, and availability, to help hosts optimize their pricing strategy and assist guests in finding appropriately priced accommodations.

## Problem Statement
The project focuses on developing a predictive model that estimates Airbnb listing prices by analyzing multiple factors that impact pricing dynamics. It provides users with insights into how different characteristics of a listing, such as its location or type of room, affect its price, empowering them with the information needed to make informed decisions.

## Dataset
The primary dataset used in this project is the New York City Airbnb Open Data available on Kaggle. It includes extensive details on Airbnb listings within NYC. Key features analyzed include:
- Neighborhood and neighborhood group
- Type of room (e.g., entire home, private room)
- Minimum number of nights required for booking
- Number of reviews and host listing counts
- Availability throughout the year
- Geographical coordinates (latitude and longitude)

## Technologies Used
- **Python**: Core programming language for data processing and model development.
- **Flask**: Lightweight WSGI web application framework used to create the web interface.
- **HTML/CSS/Bootstrap**: Used for developing the frontend, ensuring a responsive and user-friendly interface.
- **Scikit-Learn**: Employed for implementing and tuning machine learning algorithms.
- **Pandas & NumPy**: Essential libraries for efficient data manipulation and numerical computation.

## Features
- **Price Prediction**: Users can input specific details about an Airbnb listing to receive price estimates.
- **Interactive Visualizations**: The application provides dynamic visualizations that display the relationship between different features and their impact on pricing.
- **Error Handling**: Implements comprehensive form validation to ensure data integrity before submission.
