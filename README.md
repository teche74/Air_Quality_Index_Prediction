# Time Series Prediction of Air Quality (PM 2.5) in Africa/Nairobi
This project focuses on predicting air quality, specifically PM 2.5 values, in the Africa/Nairobi region using time series analysis techniques. The goal is to develop accurate models that can forecast PM 2.5 levels and provide valuable insights for environmental monitoring and public health.

## Dataset
The dataset used for this project contains historical PM 2.5 measurements in the Africa/Nairobi region. It includes hourly observations of PM 2.5 values, along with corresponding timestamps. The dataset also contains missing values that need to be addressed to ensure reliable predictions.

## Techniques and Models
Data Preprocessing
To handle missing data in the dataset, several techniques are employed:

- Forward Fill (Forward Step Validation): This method involves propagating the last available observation forward in time to fill missing values. It is particularly useful when the missing values occur in sequences, such as consecutive hours. Forward fill helps maintain temporal continuity in the dataset and ensures a consistent time series structure.
Time Series Models
Two types of time series models are applied to predict PM 2.5 values:

- Linear Model (Auto-Regressive): The linear model, specifically the Auto-Regressive (AR) model, assumes that the current value in a time series is a linear combination of past observations. By estimating the coefficients of the linear equation, the model can make predictions based on previous values. The AR model is useful for capturing patterns and trends in the time series.

- ARMA Model: The AutoRegressive Moving Average (ARMA) model combines the concepts of both auto-regression and moving average. It captures the linear relationship between the current observation and a combination of past observations, as well as the influence of random noise. The ARMA model is capable of capturing both short-term and long-term patterns in the time series.

- Hyperparameters : Hyperparameters are configuration parameters that are not learned from the data but are set prior to model training. In the context of the AR and ARMA models, the hyperparameters include:
    - AR Order: The order of the auto-regressive component, denoted as p in AR(p) models. It represents the number of lagged observations used for prediction.
    - MA Order: The order of the moving average component, denoted as q in ARMA(p,q) models. It represents the number of lagged forecast errors used for prediction.
 
## Results and Evaluation
The performance of the developed models is evaluated based on various metrics, including mean squared error (MSE), mean absolute error (MAE), and root mean squared error (RMSE). These metrics provide insights into the accuracy and precision of the predictions.

Detailed results and evaluations, including visualizations of predicted PM 2.5 values compared to actual values, are presented in the project's notebook.

## Conclusion
In this project, we successfully applied time series analysis techniques, including the linear model ,(AR)model and ARMA model, to forecast PM 2.5 values in the Africa/Nairobi region. By addressing missing data and choosing appropriate hyperparameters, we developed accurate models that can contribute to air quality monitoring and environmental management efforts.
