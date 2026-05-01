# Data Mining Projects

This repository contains three end-to-end projects demonstrating core data mining techniques, including data preprocessing, data warehousing, association rule mining, and machine learning/deep learning applications.

---

## Overview

The projects were developed as part of a Data Mining coursework and focus on applying practical techniques such as:

* Data preprocessing and feature engineering
* Data warehousing and OLAP analysis
* Association rule mining (Apriori and FP-Growth)
* Machine learning and deep learning for prediction tasks

Each project highlights a different stage of the data mining pipeline, from raw data preparation to advanced predictive modeling.

---

# Project 1: Data Preprocessing & Feature Engineering (Stroke Dataset)

## Goal

Prepare healthcare data for predictive modeling by building a robust preprocessing and feature engineering pipeline.

## Key Work

### Exploratory Data Analysis (EDA)

* Identified patterns in stroke risk factors such as age and glucose levels

### Data Cleaning

* Removed duplicates and inconsistencies
* Handled missing values using multiple imputation techniques
* Compared methods and found KNN imputation to perform best

### Outlier Handling

* Detected outliers using IQR method
* Applied transformations to reduce skewness

### Feature Engineering

* Created risk categories
* Derived age groups and ratio-based features

## Insights

* Stroke risk is strongly associated with age and glucose levels
* High-quality preprocessing is essential for reliable modeling

## Outcome

A fully cleaned, transformed, and feature-enhanced dataset ready for machine learning models.

## Tech Stack

Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

---

# Project 2: Data Warehousing & Association Rule Mining

## Goal

Design a data warehouse, perform OLAP analysis, and extract meaningful patterns from transactional data.

## Key Work

### Data Warehouse Design

* Built a PostgreSQL-based data warehouse
* Designed a snowflake schema (fact and normalized dimension tables)

### OLAP Analysis

* Executed analytical queries for:

  * Salary distribution analysis
  * Workforce trends
  * Retention rates

### Data Cube Modeling

* Constructed a multidimensional data cube (4 dimensions → 625 cuboids)
* Applied slice, roll-up, and aggregation operations

### Association Rule Mining

* Applied Apriori and FP-Growth algorithms
* Evaluated rules using support, confidence, and lift
* Identified strong product associations and co-purchasing patterns

## Insights

* Strong opportunities for cross-selling and product bundling
* FP-Growth proved more efficient than Apriori while producing identical results

## Outcome

An end-to-end analytical pipeline covering data warehousing, OLAP, and pattern mining.

## Tech Stack

Python, SQL (PostgreSQL), SQLAlchemy, Pandas, mlxtend, Seaborn

---

# Project 3: Bitcoin Price Prediction (Machine Learning & Deep Learning)

## Goal

Predict whether Bitcoin closing price will increase within the next 30 minutes using classification models.

## Problem Type

Binary classification (price up or down)

## Dataset

High-frequency BTC/USDT 1-minute trading data

## Feature Engineering

* Price-based features (returns, price ranges)
* Technical indicators (RSI, MACD, moving averages)
* Volatility and momentum signals
* Volume-based metrics

## Models Used

* Random Forest
* XGBoost
* CNN–LSTM hybrid deep learning model

## Results

* All models achieved approximately 51–52% accuracy (slightly above random baseline)
* XGBoost performed best in terms of F1-score and recall
* No significant overfitting observed

## Key Takeaways

* Short-term financial markets behave close to a random walk
* Feature engineering improves performance but has limits
* Real-world trading costs would likely eliminate small predictive edges

## Future Improvements

* Incorporate sentiment and macroeconomic data
* Apply time-series cross-validation
* Explore transformer-based temporal models

## Tech Stack

Python (Pandas, NumPy), Scikit-learn, XGBoost, TensorFlow/Keras, Matplotlib, Seaborn

---

# Summary

These projects demonstrate a full data mining pipeline:

1. Data preprocessing and feature engineering
2. Data warehousing and analytical querying
3. Pattern discovery using association rules
4. Predictive modeling with machine learning and deep learning

Together, they highlight both classical and modern approaches to data mining and applied analytics.
