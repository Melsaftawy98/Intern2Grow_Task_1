# Introduction
The goal of this project is to develop a machine learning model that predicts the price of cakes based on various features such as size, ingredients cost, design complexity, and other relevant factors. This project aims to provide a reliable tool for estimating cake prices, helping both bakers and customers to set and understand pricing.

# Dataset Overview
 
### Source: 
The dataset used in this project contains 4,000 samples with 8 features. Each sample represents a cake with various attributes:
- Sold_On: The day of the week the cake was sold.
- Size: Size of the cake (e.g., small, medium, large).
- Ingredients_Cost: Cost of ingredients used.
- Design_Complexity: Complexity of the cake's design (e.g., simple, complex).
- Time_Taken: Time taken to make the cake.
- Price: The target variable, representing the price of the cake.
- Amount: Quantity sold.
- Gender: Gender of the customer.

# Methodology
    
### Data Preprocessing

- **Encoding Categorical Variables:** The categorical variables Sold_On, Size, and Design_Complexity were encoded using one-hot encoding. The Gender variable was mapped to binary values (female = 1, male = 0).

- **Feature Scaling:** Numerical features such as Ingredients_Cost, Time_Taken, and Amount were normalized using MinMaxScaler to bring all values into the range [0, 1].

### Model Training

- **Model Used:** A Linear Regression model was employed to predict the price of cakes.

- **Training and Testing Split:** The dataset was split into training (80%) and testing (20%) sets using train_test_split.

- **Model Evaluation:** The model was evaluated using metrics such as R-squared (R²), Root Mean Squared Error (RMSE), and Mean Absolute Error (MAE).

# Results

### Model Performance:
- **R-squared:** The model achieved an R-squared value of 0.974, indicating that it explains 97.4% of the variance in the price data.
- **RMSE:** The Root Mean Squared Error was 11.897, showing that, on average, the predictions are within 11.9 units of the actual prices.
- **MAE:** The Mean Absolute Error was 9.744, reflecting the average absolute difference between the predicted and actual prices.

# Conclusion
The Linear Regression model performs well in predicting cake prices, with high accuracy as reflected by the R-squared value. The relatively low RMSE and MAE further suggest that the model's predictions are close to the actual prices. These results indicate that the model could be effectively used in real-world applications to assist in cake pricing.

# Future Work
While the model shows strong performance, future work could involve exploring more advanced regression techniques, feature engineering, and hyperparameter tuning to possibly improve the accuracy even further.
