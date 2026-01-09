---
title: "US Rent Price Predictor"
excerpt: "Machine learning model to predict rental prices across the US using 300k+ Craigslist listings. Features Streamlit dashboard for interactive price estimation."
collection: project
image: "/images/user-interface_project4.png"
tags:
  - Machine Learning
  - Streamlit
  - Python
  - Data Science
github: "https://github.com/Nirmalyan/us_rent_price_prediction"
---

# US Rent Price Prediction 

The goal of this project is to analyze rental postings across the United States and provide actionable insights through graphs and an intuitive user interface.

## Problem Statement 

While supply and demand is a major factor influencing rental prices, several factors such as parking, location, housing type, and pet policies can cause fluctuations. This project helps understand these anomalies and how they change over time with respect to demographics.

## Dataset

- **Source**: [Kaggle - USA Housing Listings](https://www.kaggle.com/austinreese/usa-housing-listings)
- **Size**: 300k+ listings from Craigslist
- **Features**: 22 attributes including location, amenities, and property details

## Key Findings

- Decision Tree Regression outperformed Gradient Boosting and Linear Regression
- Key features: sqfeet, beds, baths
- Location significantly impacts price (California, Massachusetts, Hawaii)

## Tech Stack

- **ML**: Scikit-learn, XGBoost
- **Visualization**: Matplotlib, Seaborn
- **Web App**: Streamlit
- **Database**: SQLite

## Features

- Interactive price prediction
- Feature importance visualization
- Geographic analysis
- Trend analysis over time
