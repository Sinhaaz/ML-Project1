## Project Name :- Student Performance Indicator
# Project Name :- Student Performance Indicator

# Approach :-
- Data Ingestion :
  In Data Ingestion phase the data is first read as csv.
  Then the data is split into training and testing and saved as csv file.
## Approach :-
1. Data Ingestion :
   - In Data Ingestion phase the data is first read as csv.
   - Then the data is split into training and testing and saved as csv file.

- Data Transformation :
  In this phase a ColumnTransformer Pipeline is created.
  for Numeric Variables first SimpleImputer is applied with strategy median , then Standard Scaling is performed on numeric data.
  for Categorical Variables SimpleImputer is applied with most frequent strategy, then ordinal encoding performed , after this data is scaled with Standard Scaler.
  This preprocessor is saved as pickle file.
2. Data Transformation :
   - In this phase a ColumnTransformer Pipeline is created.
   - for Numeric Variables first SimpleImputer is applied with strategy median , then Standard Scaling is performed on numeric data.
   - for Categorical Variables SimpleImputer is applied with most frequent strategy, then ordinal encoding performed , after this data is scaled with Standard Scaler.
   - This preprocessor is saved as pickle file.

- Model Training :
  In this phase base model is tested . The best model found was catboost regressor.
  After this hyperparameter tuning is performed on catboost and knn model.
  A final VotingRegressor is created which will combine prediction of catboost, xgboost and knn models.
  This model is saved as pickle file.
3. Model Training :
   - In this phase base model is tested . The best model found was catboost regressor.
   - After this hyperparameter tuning is performed on catboost and knn model.
   - A final VotingRegressor is created which will combine prediction of catboost, xgboost and knn models.
   - This model is saved as pickle file.

- Prediction Pipeline :
  This pipeline converts given data into dataframe and has various functions to load pickle files and predict the final results in python.
4. Prediction Pipeline :
   - This pipeline converts given data into dataframe and has various functions to load pickle files and predict the final results in python.

## Screenshot :-
<img src = "Screenshot.jpg">