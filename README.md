# Real-Estate-Price-Predictor-and-Recommendation-System

This project involves predicting the prices of flats and houses based on various parameters, performing data analysis, and providing recommendations based on location and similarity scores. The project is implemented using a Flask app for demonstration purposes.

## Table of Contents

- [Introduction](#introduction)
- [Project Components](#project-components)
  - [Price Prediction](#price-prediction)
  - [Analytics Module](#analytics-module)
  - [Recommender System](#recommender-system)
- [Data Collection and Preparation](#data-collection-and-preparation)
- [Feature Engineering and EDA](#feature-engineering-and-eda)
- [Model Training](#model-training)
- [Recommender Systems](#recommender-systems)
- [Streamlit Application](#streamlit-application)
- [Results](#results)

## Introduction

The goal of this project is to predict the prices of real estate properties and provide analytical insights and recommendations to potential buyers. The project is divided into three main components: price prediction, analytics module, and a recommender system.

## Project Components

### Price Prediction

The price prediction model estimates the price of a flat or house based on the following parameters:
- Built-up area
- Number of bedrooms
- Number of bathrooms
- Furnishing category
- Luxury score
- Property type
- Sector
- Number of Balconies
- Property Age
- Servant Room
- Store Room
- Floor Category

The model is trained using a Random Forest algorithm and achieves an R2 score of 0.9023.

### Analytics Module

The analytics module provides various visualizations to help understand the data, including:
- Sector-wise price per sqft geomap
- Side-by-side distribution plots of flats and houses
- Feature Wordcloud
- Area vs Price scatter plot
- Number of Bedroom pie chart and corresponding price comparison

### Recommender System

The recommender system has two components:
1. *Location-based Recommendation*: Provides recommendations based on the location and a chosen radius.
2. *Similarity-based Recommendation*: Provides recommendations based on similarity scores between flats. This includes:
   - Landmarks similarity
   - Facilities similarity
   - Price similarity
     The final recommender system combines the results of these three systems.

The final recommendation is a combination of these three systems, with different importance assigned to each aspect.

## Data Collection and Preparation

* Data was web-scraped from 99acres and other real estate websites.
* Ensured diversity and comprehensiveness in the dataset.
* Addressed missing values and inconsistencies.
* Unified datasets of flats and houses for seamless analysis.

## Feature Engineering and EDA

* Added new features such as luxury scores, additional room indicators, and area-type combinations.
* Conducted univariate and multivariate analyses using Pandas Profiling.
* Addressed outliers and imputed missing data in critical columns.
* Feature selection techniques included SHAP, LASSO, and Random Forest Feature Importance.

## Model Training

The cleaned data was used to train a Random Forest model to predict property prices. The model achieved an R2 score of 0.9023, indicating a high level of accuracy.

The final recommender system combines the results of these three systems.

## Streamlit Application

The project is demonstrated using a Streamlit Application with a Sidebar for each functionality. Users can:
- Predict property prices.
- Explore analytical insights through interactive visualizations.
- Access personalized property recommendations.

The app design emphasizes simplicity and functionality, ensuring a seamless user experience.

## Results

The project achieves the following outcomes:

* High Prediction Accuracy: The Random Forest model achieves an R² score of 0.9023.
* Comprehensive Market Insights: Interactive analytics provide actionable insights into property trends.
* Tailored Recommendations: The recommender system offers location-based and similarity-driven suggestions.
This solution empowers users to make informed decisions in the real estate market with confidence.

### User Interface
![FireShot Capture 002 - 🏠 Real Estate Price Predictor   Recommendation Tool - localhost](https://github.com/user-attachments/assets/91d0ac8d-bc8e-4a0d-b2de-caefa64fb95c)

### Price Prediction
![FireShot Capture 003 - 🏡 Property Price Prediction - localhost](https://github.com/user-attachments/assets/12354cb0-dba8-4338-a80e-33995544c389)

### Analytics Module
![FireShot Capture 006 - Plotting Demo - localhost](https://github.com/user-attachments/assets/c9408fbf-43e0-4d3c-8f67-7aad22831a9e)

### Recommendation System
![FireShot Capture 004 - Recommend Apartments - localhost](https://github.com/user-attachments/assets/122e7305-4d44-40a4-861a-2a0617a877e0)
