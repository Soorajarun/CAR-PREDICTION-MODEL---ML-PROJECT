# CAR-PREDICTION-MODEL ML-PROJECT
This machine learning algorithm uses regression to forecast car prices. 
Project Report: Introduction to the Car Price Prediction Model This project's goal was to create a machine learning model that could precisely forecast auto prices. To help manufacturers understand pricing dynamics, we investigated links between different automotive characteristics and their prices using the car price dataset. To find the optimal regression model, this required data cleaning, preprocessing, exploratory data analysis, model construction, and evaluation.
Dataset and Preprocessing Details:
The dataset included a variety of variables, such as pricing and vehicle details. Null values, duplicates, skewed features, and outliers were discovered during the initial data analysis.

Preprocessing Steps:To maintain data integrity, duplicates and missing values were handled. Numerical features' skewness was fixed by using square root and logarithmic transforms. Box plots, the IQR method, and capping approaches were used to identify and handle outliers.
Feature Engineering: One-Hot and Label Encoding techniques were used to encode categorical information. To keep only significant predictors, the Variance Threshold technique was used to select significant features.
Analysis of Exploratory Data (EDA) Relationships and distributions in the data were examined using visualizations such bar charts, scatter plots, correlation matrices, and histograms. Key characteristics that were highly connected with the target variable (price) were found using a correlation matrix.
Development of Models Multiple regression models were constructed to forecast car prices once the dataset was divided into training and testing sets. The models listed below were put into practice and assessed:
Model R² Score MAE RMSE Linear Regression 0.8257 0.1616 0.2018 Decision Tree Regressor 0.7450 0.1709 0.2441 Random Forest Regressor 0.8762 0.1366 0.1700 Gradient Boosting Regressor 0.8912 0.1337 0.1594 Support Vector Regressor 0.7909 0.1779 0.2210
Gradient Boosting Regressor emerged as the best model based on its superior R² score and lower error metrics.

Model Evaluation and Hyperparameter Tuning Model Evaluation:

Actual vs. Predicted prices were visualized using scatter plots with a trend line to assess model performance. Gradient Boosting Regressor showed the closest alignment between predicted and actual values. Hyperparameter Tuning:

The Gradient Boosting Regressor was optimized using GridSearchCV, improving its performance further. Final tuned model test results: R² Score: 0.9089 MAE: 0.12 RMSE: 0.15

Model Deployment The final Gradient Boosting Regressor model was saved for future use, enabling its integration into production systems for price prediction tasks.

Conclusion This project successfully developed a robust regression model for car price prediction. Key highlights include:

Comprehensive preprocessing ensured data quality. Gradient Boosting Regressor was identified as the best-performing model, achieving high accuracy with an R² score of 0.9089 on the test set. Hyperparameter tuning further enhanced model performance. This model can help car manufacturers understand pricing dynamics and make data-driven decisions regarding design and market strategy. Future work could explore advanced ensemble methods, additional feature engineering, or the inclusion of real-time market data for further improvement.
