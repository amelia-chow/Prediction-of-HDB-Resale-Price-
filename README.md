# 🏠HDB Resale Price Prediction

## Project Overview
This mini project aims to analyses HDB resale flat data to explore factors affecting resale prices and predict HDB flat resale prices in Singapore. 
The project combines exploratory data analysis, clustering, and regression modelling to uncover patterns in the data and evaluate predictive performance.

## 📝Project Objectives

- Explore key factors influencing HDB resale prices
- Identify patterns and relationships between housing characteristics and price
- Segment flats into clusters based on selected features
- Build and compare machine learning models for resale price prediction

## Dataset

The dataset consists of historical data from **January 2017 to March 2026** and includes variables related to HDB resale flats, such as:

- `resale_price`
- `floor_area_sqm`
- `hdb_age`
- `storey_range`

Full csv file: [HDB resale prices flat](resale_flat_prices.csv)

## 🛠️Tools and Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## 📁Project Workflow

### 1.🧹 Data Cleaning and Preparation
- Checked for missing values and data types
- Converted variables into suitable formats for analysis
- Transformed `storey_range` into a numeric midpoint value

### 2.📈Exploratory Data Analysis (EDA)
- Analysed the distribution of resale prices
- Studied relationships between resale price and features such as HDB age, floor area, Town
- Used visualisations such as histograms, scatter plots, box plots, and correlation matrices

### 3. Clustering
- Applied K-means clustering to segment flats based on selected features:
  - `floor_area_sqm`
  - `hdb_age`
  - `storey_midpoint`
- Used the elbow method to determine the optimal number of clusters
- Compared resale price distributions across clusters

### 4. Predictive Modelling
The following regression models were built and evaluated:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

### 5. Model Evaluation
Models were evaluated using:
- **R² score**
- **Mean Squared Error (MSE)**

## Key Results

- Both **Random Forest** and **Linear Regression** achieved strong predictive performance on the testing set
- Random Forest achieved a perfect fit on the training set, which may suggest slight overfitting
- Linear Regression showed more consistent performance between training and testing sets


Full code: [HDB resale prices](HDB_resale_prices.ipynb)
