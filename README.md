# Rent Price Prediction in Canada

## Overview
This project focuses on predicting rent prices across Canada by leveraging regression techniques to analyze various features of rental properties. The dataset includes information on the province, square footage, number of bedrooms and bathrooms, and pet policies. The project explores different modeling approaches, including polynomial regression and interaction terms, to capture the complex relationships between features. After encountering issues with multicollinearity and model performance, RidgeCV regression was used as a final step to improve prediction accuracy and stability.

## Data Features
- 'rentfaster_id' - id of property on https://www.rentfaster.com . Can be explore with www.rentfaster.ca/rentfaster_id
- 'city' - city of property like 'Toronto', 'Calgary', 'Vancuver' and etc.
- 'province' - province of property like 'Alberta', 'Ontario' and etc.
- 'address' - address of property like '333 Seymour St' and etc
- 'latitude' - latitude coordinate of rental property
- 'longitude' - longitude coordinate of rental property
- 'lease_term' - category of rental period like 'Long Term', 'Negotiable' and etc
- 'type' - category of type a rental property like 'House', 'Apartment', 'Basement' and etc
- 'price' - price in CAD
- 'beds' - count of bedrooms
- 'baths' - count of bathrooms
- 'sq_feet' - area of rental property in square feets
- 'link' - right side of url for getting full details of the property rentfaster.com+'link'
- 'furnishing' - Furnished or not
- 'availability_date' - Date of availability
- 'smoking' - is allow smoke
- 'cats' - is allow cats
- 'dogs' - is allow dogs

## Dataset
You can download the dataset from the following link: [rentfaster.csv](https://www.kaggle.com/datasets/sergiygavrylov/25000-canadian-rental-housing-market-june-2024)

## Approach
1. **Initial Polynomial Regression:** The first step involved applying polynomial regression to capture non-linear relationships between the features and rent prices.
2. **Adding Interaction Terms with LassoCV:**  Interaction terms were introduced to explore how combinations of features might affect rent prices. LassoCV was used during this phase to perform feature selection and regularization. While this approach aimed to enhance model accuracy, it led to an increase in RMSE (Root Mean Square Error) and high Variance Inflation Factor (VIF) values, signaling multicollinearity.
3. **Feature Selection and Multicollinearity:** To address the high VIF values, features with excessive multicollinearity were removed.
4. **RidgeCV Regression:**  To further refine the model and handle multicollinearity, RidgeCV regression was employed. This method applies regularization to stabilize coefficients and enhance model performance.

## Conclusion
This project demonstrates the use of various regression techniques and feature engineering strategies to predict rent prices. RidgeCV was effective in managing multicollinearity and improving the overall model performance.

