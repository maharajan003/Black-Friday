Black Friday Sales Prediction using Random Forest Regressor
Project Overview :
This project aims to predict the purchase amounts during Black Friday sales based on customer demographics and product details. The goal is to build a model that accurately estimates how much a customer is likely to spend, which can help retailers optimize their sales strategies and inventory management.

Problem Statement:
Given a dataset containing customer demographics, product details, and purchase amounts, the task is to build a predictive model using the Random Forest Regressor to forecast future purchases during Black Friday sales.

Dataset:
The dataset used for this project includes the following features:

User_ID: Unique identifier for each customer.
Product_ID: Unique identifier for each product.
Gender: Gender of the customer.
Age: Age group of the customer.
Occupation: Occupation code of the customer.
City_Category: Category of the city (A, B, C).
Stay_In_Current_City_Years: Number of years the customer has stayed in the current city.
Marital_Status: Marital status of the customer.
Product_Category_1, 2, 3: Categories of the products purchased.
Purchase: Amount spent on the purchase (target variable).

Key Concepts:
1. Data Preprocessing:
  Handling Missing Values: Missing values in product categories were handled by filling them with zeros or the median of the category.
  Feature Engineering: Created new features such as total product categories purchased and combined product categories into broader     
  groups for better prediction.
2. Exploratory Data Analysis (EDA):
  Understanding Data Distribution: Visualized the distribution of numerical features like age, purchase amount, and product categories.
  Correlation Analysis: Analyzed the correlation between different features and the target variable to identify significant predictors.
  Customer Segmentation: Segmented customers based on demographics and spending patterns to understand purchasing behavior.
3. Modeling with Random Forest Regressor:
  Why Random Forest?: Random Forest was chosen due to its robustness, ability to handle large datasets with higher dimensionality, and  
  its effectiveness in reducing overfitting by averaging multiple decision trees.
  Model Training: The model was trained using the Random Forest Regressor, which involves constructing multiple decision trees during     
  training and outputting the mean prediction of the individual trees.
  Hyperparameter Tuning: Used GridSearchCV to optimize the key hyperparameters such as the number of trees (n_estimators), maximum depth 
  of trees (max_depth), and minimum samples required to split a node (min_samples_split).
4. Model Evaluation:
Evaluation Metrics: The model's performance was evaluated using the Root Mean Squared Error (RMSE) metric, which measures the average 
  magnitude of the error between predicted and actual purchase amounts.
Results: The final model achieved an RMSE of 3055.58, indicating the model's predictive accuracy.
5. Conclusion:
   The Random Forest Regressor model demonstrated solid predictive performance and provided insights into customer purchasing behavior.      The model can be further refined by experimenting with additional feature engineering and hyperparameter tuning.
6. Future Work:
Feature Importance Analysis: Analyze the importance of different features to understand which customer or product attributes have the 
   most significant impact on purchasing behavior.
Ensemble Methods: Explore other ensemble methods or stacking techniques to improve predictive performance.
Deployment: Deploy the model as a web application to predict purchase amounts in real-time.
