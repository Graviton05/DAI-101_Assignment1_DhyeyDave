# DAI-101_Assignment1_DhyeyDave
# Forest Fire Data Analysis

# Variables Information
1. X - x-axis spatial coordinate within the Montesinho park map: 1 to 9
2. Y - y-axis spatial coordinate within the Montesinho park map: 2 to 9
3. month - month of the year: 'jan' to 'dec' 
4. day - day of the week: 'mon' to 'sun'
5. FFMC - FFMC index from the FWI system: 18.7 to 96.20
6. DMC - DMC index from the FWI system: 1.1 to 291.3 
7. DC - DC index from the FWI system: 7.9 to 860.6 
8. ISI - ISI index from the FWI system: 0.0 to 56.10
9. temp - temperature in Celsius degrees: 2.2 to 33.30
10. RH - relative humidity in %: 15.0 to 100
11. wind - wind speed in km/h: 0.40 to 9.40 
12. rain - outside rain in mm/m2 : 0.0 to 6.4 
13. area - the burned area of the forest (in ha): 0.00 to 1090.84

This project analyzes a dataset of forest fires to understand the factors influencing their occurrence and spread.


## Data Cleaning and Preprocessing

- **Handling Missing Values:** Missing values in the dataset were addressed using mean imputation for numerical features ('FFMC') and mode imputation for categorical features ('rain', 'area').
- **Data Type Conversion:** Categorical features ('month', 'day') were converted to the appropriate data type.
- **Outlier Handling:** Outliers in numerical features ('rain', 'area') were removed using the Interquartile Range (IQR) method.
- **Duplicate Removal:** Duplicate rows were identified and removed from the dataset.

## Exploratory Data Analysis (EDA)

- **Univariate Analysis:** Distributions of individual features were examined using histograms and descriptive statistics for numerical features and countplots for categorical features.
- **Bivariate Analysis:** Relationships between pairs of features were explored using scatter plots for numerical features and box plots for categorical vs. numerical features.
- **Multivariate Analysis:** Correlations between multiple numerical features were analyzed using a correlation matrix of pearson coefficient and visualized with a heatmap.

## Feature Engineering and Selection

- **Feature Removal:** The 'rain' feature was removed due to its insignificant impact on the target variable ('area').

## Further Analysis (Potential Next Steps)

- **Predictive Modeling:** Building machine learning models to predict the area affected by forest fires based on the identified factors.
- **Data Visualization:** Creating interactive visualizations to gain deeper insights into the data.
- **Geospatial Analysis:** Incorporating geographical information to analyze spatial patterns of forest fires.
