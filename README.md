# Real Estate Price Prediction
## Overview 
This project focuses on predicting real estate prices using machine learning. Starting with a dataset from Kaggle, we cleaned and prepared the data to improve accuracy, then built and compared models like Ordinary Least Squares (OLS), Ridge, and Lasso regression. The final result is an interactive tool that lets users estimate property prices based on their preferences, making it easier to explore options and understand the housing market.

## Features
- Predict real estate prices with 94.94% accuracy using Ordinary Least Squares (OLS) regression.
- Conduct comparative analysis of Ridge (94.91%) and Lasso (94.93%) regressions to tackle multicollinearity and perform feature selection.
- Build an interactive tool that generates real-time price predictions based on user-defined property preferences. 

## Technologies Used
- **Python**: Core programming language.
- **Pandas**: Data manipulation and preprocessing.
- **NumPy**: Numerical computations.
- **scikit-learn**: Model training, evaluation, and optimization.

## Dataset 
- **Source**: [Housing Prices Regression](https://www.kaggle.com/datasets/denkuznetz/housing-prices-regression) on Kaggle.
- **Description**: This dataset provides key factors driving real estate prices, suitable for regression analysis.
- **Features**: Square footage, number of bedrooms, number of bathrooms, number of floors, year built, presence of amenities (garden, pool), garage size, location score, and distance to city center.
    - Has_Garden: Indicates the presence (1) or absence (0) of a garden.
    - Has_Pool: Indicates the presence (1) or absence (0) of a pool.
    - Garage_Size: Size of the garage in square feet.
    - Location_Score: A numerical score representing the desirability of the property's location.
  
# Project Workflow 
  ## Data Preprocessing
  - **Cleaning**:
      - Removed irrelevant columns, such as ID.
      - Handled missing values and outliers to ensure data quality.
  - **Feature Engineering**:
      - Calculated Age of the property as 2024 - Year_Built.
      - Standardized numerical features to improve model performance.
   
  ## Model Performance
  - **Ordinary Least Squares (OLS) Regression**:
      - Achieved an R-Squared value of 0.9494, indicating that approzimatelyy 94.94% of the variance of property prices is explained by the model.
  - **Ridge Regression**:
      - R-squared value: 0.9491
      - Utilized to address potential multicollinearity among features.
  - **Lasso Regression**:
      - R-squared value: 0.9493
      - Utilized for feature selection by shrinking less important feature coefficients to zero. 
  ## Interactive Tool 
  Developed a user-friendly interfact where users can input property specifications to receive real-time price predicitions. The tool utilizes the trained regression models to provide accurate and immediate estimates.
  ## Future Enhancements 
  - **Data Enrichment**: Incorporate additional features such as neighborhood amenities, school district ratings, and crime statistics to improve model accuracy.
  - **Model Optimization**: Explore advanced regression techniques and ensemble methods to enhance predictive performance.


