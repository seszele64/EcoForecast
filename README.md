EcoForecast is a data-driven project designed to explore the relationship between weather conditions and renewable energy production in Poland. Utilizing historical weather data from 25 different stations and corresponding daily renewable energy output statistics for the year 2022, this project aims to uncover patterns and trends that influence the renewable energy sector. Through sophisticated data analysis and machine learning techniques, EcoForecast seeks to predict future renewable energy outputs based on forecasted weather conditions, thereby providing valuable insights for energy management and policy-making. This initiative not only helps in optimizing the use of renewable resources but also supports sustainable development goals by enhancing the predictability and reliability of renewable energy sources.

### Research Summary

**Objective:** The project's primary goal is to model and predict the percentage of renewable energy production using weather-related variables from various stations across Poland.

### Methodology

1. **Data Preparation:**
   - **Data Splitting:** The dataset was divided into training (80%) and testing (20%) sets using scikit-learn's `train_test_split`.
   - **Variable Selection:** Predictors included various weather-related features, with 'RenewablePercentage' as the target variable.

2. **Model Development:**
   - **Model Choice:** A RandomForestRegressor was employed due to its ability to handle non-linear relationships and feature interactions.
   - **Training:** The model was trained on the training dataset with parameters optimized for generalization.

3. **Model Evaluation:**
   - **Metrics:** Evaluation included Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared.
   - **Results:** The model achieved an MAE of 1.22, MSE of 2.98, RMSE of 1.73, and an R-squared of 0.95, indicating excellent predictive accuracy.

4. **Feature Importance Analysis:**
   - **Key Predictors:** Avg_Wind_Speed was the most significant predictor, highlighting its crucial role in predicting renewable energy outputs. Other important predictors included Avg_Max_Temp and Avg_Cloudiness.

5. **Visualization:**
   - **Predictive Accuracy:** A scatter plot of actual vs. predicted values showed a high degree of alignment, with most data points clustering close to the identity line (y=x), reinforcing the model's accuracy.

### Insights and Conclusions

- The RandomForest model effectively captured the relationships between weather conditions and renewable energy outputs.
- Wind speed emerged as a critical factor, likely due to its direct influence on wind energy production, a significant component of renewable energy in Poland.
- The high R-squared value suggests that the model could explain most of the variability in the renewable energy outputs, affirming the strong influence of selected weather variables.
- The findings could aid in optimizing energy production and planning, contributing to more efficient and reliable renewable energy use.

This summary encapsulates the scope, methods, results, and implications of your research, presenting a clear picture of your project's contributions and potential impact.
