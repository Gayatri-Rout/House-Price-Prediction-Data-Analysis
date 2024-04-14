# House-Price-Prediction-Data-Analysis

## Introduction

This report presents an exploratory data analysis (EDA) of a dataset related to house prices. The dataset was obtained from [Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data).

## Data Overview

The dataset consists of 1460 records and 81 features. These features include both numerical and categorical variables, such as lot frontage, house size, neighborhood, and more. Before proceeding with the analysis, missing values were handled, outliers were identified, and feature engineering techniques were applied to preprocess the data.

## Missing Values

- The dataset contains missing values in several features, with varying percentages of missingness ranging from less than 1% to almost 100%.
  ![image](https://github.com/Gayatri-Rout/House-Price-Prediction-Data-Analysis/assets/70259060/fd570f94-0762-4bac-b2f3-35baf434219c)
  
- The graphs showed some relationship between the missing values and sale price. Thus all these features are important for prediction and can't be dropped.
- Missing values were imputed or replaced using appropriate techniques, such as filling with median values for numerical features and replacing with a new label for categorical features.

## Numerical Variables

### Discrete Variables

- 17 discrete variables were identified, including features like the overall quality of the house, the number of rooms, and the number of bathrooms.
- The relationship between discrete variables and the sale price was visualized using bar plots.
  ![image](https://github.com/Gayatri-Rout/House-Price-Prediction-Data-Analysis/assets/70259060/2f613a3e-00f8-4bf9-81f3-c9a98dcb9b5a)
  ![image](https://github.com/Gayatri-Rout/House-Price-Prediction-Data-Analysis/assets/70259060/de51fb83-448d-45f5-a735-1f5ca9476a54)

### Continuous Variables

- 16 continuous variables were identified, such as lot area, living area, and garage area.
- The distribution of each continuous variable was visualized using histograms, and it is clear that the data is skewed.
  ![image](https://github.com/Gayatri-Rout/House-Price-Prediction-Data-Analysis/assets/70259060/b42b7d28-2efb-408b-8abc-94549afc73e5)
  - Logarithmic transformation was applied to transform skewed data to approximate normality.
  ![image](https://github.com/Gayatri-Rout/House-Price-Prediction-Data-Analysis/assets/70259060/104a16db-e03f-4898-a295-bd3299817ba9)
  -  Outliers in continuous variables were identified using box plots to understand their impact on the data distribution.
  ![image](https://github.com/Gayatri-Rout/House-Price-Prediction-Data-Analysis/assets/70259060/6692dd47-8dd5-4649-b7ac-25fd53b7ade7)

### Temporal Variables

- Year-related variables, such as the year the house was built or remodeled, were analyzed to understand their relationship with the sale price over time.
  ![Untitled](https://github.com/Gayatri-Rout/House-Price-Prediction-Data-Analysis/assets/70259060/34871bc6-e1b0-42e1-b9fd-0881e6d10012)
- The graph shows that the price of the house decreases with time.
- Scatter plots were used to compare the difference between each year-related variable and the year the house was sold, revealing potential trends or patterns.
  ![image](https://github.com/Gayatri-Rout/House-Price-Prediction-Data-Analysis/assets/70259060/ff64ed24-4671-46d2-8425-ca63ce5523f9)


## Categorical Variables

- The dataset contains numerous categorical variables representing features like zoning, street type, and building type.
- The relationship between categorical features and the sale price was visualized using bar plots.
  ![image](https://github.com/Gayatri-Rout/House-Price-Prediction-Data-Analysis/assets/70259060/af3818aa-5dd1-40d9-9cdc-e345eb3b39b2)

## Feature Engineering

- Rare categories in categorical features were identified and grouped into a single category to simplify the analysis.
- Categorical features were converted into numerical representations using mean encoding to prepare the data for modeling.

## Feature Scaling

- Finally, feature scaling was performed to scale numerical features to a common range using MinMaxScaler, ensuring that all features contribute equally to the analysis and modeling process.

