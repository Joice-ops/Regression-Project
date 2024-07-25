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
