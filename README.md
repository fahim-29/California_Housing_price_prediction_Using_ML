# California_Housing_price_prediction_Using_ML

The primary goal of this project was to build a machine learning model that could predict house prices in California based on factors such as location, population, income, and housing characteristics

Before training the machine learning models, I performed several data preprocessing steps to ensure high-quality data. These included:"
Handling missing values by filling total_bedrooms with the median 
Scaling numerical features to bring them to a similar range
Encoding categorical data like ocean_proximity using one-hot encoding
Feature engineering by creating new features such as rooms_per_household and bedrooms_per_room, which improved model performance.


Machine Learning Model Used
I experimented with multiple algorithms to find the best-performing model for predicting house prices. The models tested were

🔹 Linear Regression – A simple model that finds a linear relationship between features and prices. While interpretable, it didn’t perform well due to non-linearity in the data.

🔹 Decision Tree Regressor – A tree-based model that splits data at different thresholds. It captured complex patterns but tended to overfit.

🔹 Random Forest Regressor – The best-performing model! This is an ensemble learning technique that builds multiple decision trees and averages their predictions, reducing overfitting and improving accuracy.

🔹 Gradient Boosting Regressor – A boosting technique that builds models sequentially, improving predictions step by step. It was effective but computationally expensive.

 Best Model: Random Forest Regressor
 After evaluating all models, the Random Forest Regressor was selected as the best model due to its superior performance and accuracy. Some key hyperparameters I used include:
 
    •	
max_features = "sqrt" (each tree considers only a subset of features)
max_depth = 75 (to prevent overfitting)
random_state = 42 (for reproducibility)
This model provided the most reliable and accurate house price predictions.


To evaluate the models, I used three key metrics:

•	Mean Absolute Error (MAE) – Measures the average error in predictions.
•	Mean Squared Error (MSE) – Penalizes larger errors more than MAE.
• R-Squared Score (R²) – Measures how well the model explains variations in house prices.

•	"The Random Forest Regressor achieved the highest R² score, meaning it explained most of the variance in house prices, making it the best model for this dataset."



