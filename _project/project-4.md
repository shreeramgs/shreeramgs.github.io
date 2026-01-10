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

<div style="display: flex; justify-content: center; margin-bottom: 2em;">
  <div 
    style="
      background: #fff;
      border-radius: 16px;
      box-shadow: 0 2px 16px 0 rgba(0,0,0,0.17);
      padding: 2em 2em 1.5em 2em;
      max-width: 720px;
      width: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;
    "
  >
    <img 
      id="us-rent-price-img"
      src="/images/user-interface_project4.png" 
      alt="US Rent Price Predictor" 
      style="max-width: 480px; width: 90%; height: auto; border-radius: 12px; box-shadow: 0 2px 8px 0 rgba(0,0,0,0.10); margin-bottom: 1em; transition: opacity 0.5s;"
    />
    <h2 style="margin: 0.5em 0 0.2em 0; font-size: 1.5em;">US Rent Price Predictor</h2>
    <p style="color: #444; margin: 0 0 0.5em 0; font-size: 1em; text-align: center;">
      Machine learning model to predict rental prices across the US using 300k+ Craigslist listings. Features Streamlit dashboard for interactive price estimation.
    </p>
  </div>
</div>

### Description
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
