# food delivery time prediction


## Objective:
The goal of this project is to develop regression models that can predict food delivery times based on various factors such as weather conditions, restaurant location, delivery person details, and order timings.

## Dataset:
The project uses the Food Delivery Dataset, which contains information about food deliveries, including weather conditions, restaurant location, delivery person details, and order timings.

## Data Cleaning:
The dataset was cleaned by replacing missing values with appropriate values and converting data types of certain columns to ensure consistency and accuracy in the analysis.

## Feature Extraction:
Features such as city code, time taken, and various date-time features were extracted from existing columns. Additionally, the distance from the restaurant feature was extracted using the geopy library to incorporate geographical information into the models.

## Data Transformation:
Categorical columns were encoded, and numeric columns were scaled using pipelines and transformers to prepare the data for modeling.

## Modeling:
Several regression models were built, including Linear Regression, Decision Tree, Random Forest, Ridge Regression, Lasso Regression, and XGBoost. These models were chosen for their ability to handle both linear and nonlinear relationships in the data.

## Hyperparameter Tuning:
GridSearchCV was used for hyperparameter tuning and cross-validation to optimize the performance of the models.

## Model Evaluation:
The models were evaluated using R-squared as the metric, which measures the proportion of the variance in the dependent variable that is predictable from the independent variables. The R-squared scores achieved were: XGBoost Regressor (0.82), Decision Trees (0.77), and Random Forests (0.82).

## Model Saving:
The best performing models (XGBoost, Random Forest, and Decision Tree) along with the processed data were saved using joblib for future use or deployment.

## Conclusion:
The regression models developed in this project showed promising results in predicting food delivery times based on various factors. Further analysis could include feature importance analysis to identify the most influential factors affecting delivery times.
