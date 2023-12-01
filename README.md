# Predicting Flight Prices using Gradient Boosting Regressor with features including airline, source city, departure time, stops, arrival time, destination city, class, duration, and days_left using PySpark’s MLlib

## Notebook: 
https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/5691159305297624/1572755136265826/841451422945549/latest.html

## Model Overview:
 - Model Type: Gradient Boosting Regressor
 - Features Used: Airline, Source City, Departure Time, Stops, Arrival Time, Destination City, Class, Duration, Days Left
 - Framework: PySpark’s MLlib

## Model Performance Analysis:
Price Prediction Pattern: The model exhibits a linear correlation between actual and predicted flight prices, consistent up to approximately INR 70,000. However, there might be deviations beyond this price range.

<img src="https://github.com/LarryChenCode/flight_fare_prediction_using_pyspark_mllib/blob/main/prediction%20vs%20actual.png" width="700" />

## Accuracy Metrics:
 - RMSE (Root Mean Square Error): 1520.00 - Indicates a relatively small average prediction error, suggesting good model precision.
 - R² (Coefficient of Determination): 0.995 - Demonstrates that the model accounts for approximately 99.5% of the variance in the observed data, indicating high predictive power.
 - MAE (Mean Absolute Error): 601.44 - Provides an additional perspective on the average magnitude of the errors in predictions.

## Model Parameters:
 - Best Parameters Identified:
   - Number of Trees: 60
   - Number of Features: 3

## Conclusion:
The Gradient Boosting Regressor model shows a high degree of accuracy in predicting flight prices within the considered feature set. The excellent R² score coupled with a low RMSE and MAE reflects the model's effectiveness. While the model's predictions are mostly linear up to a certain price point, a slight deviation for higher-priced flights is noted, suggesting an area for further investigation and potential refinement of the model.
