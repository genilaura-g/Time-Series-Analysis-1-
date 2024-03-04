# Time-Series-Analysis-1-
Using dataset from JP Morgan X Forager - Quantative Research 

Price a Commodity Storage Contract with Time Series Analysis
This project demonstrates the application of financial market concepts and time series analysis techniques to price a commodity storage contract.

Functionality:

Reads commodity price data from a CSV file (data source not specified).
Cleans and organizes the data.
Performs exploratory data analysis (EDA) to understand trends, patterns, and price behavior.
Utilizes statistical methods to assess stationarity and model the time series data.
Implements a SARIMA (Seasonal Autoregressive Integrated Moving Average) model for price forecasting.
Evaluates the model's performance using Mean Squared Error (MSE).
Instructions:

Replace "" in data = pd.read_csv("") with the actual path to your CSV file containing commodity price data.
Ensure the data includes columns for 'Dates' and 'Prices'. Dates should be formatted appropriately for time series analysis.
Data Exploration & Visualization:

The code performs basic data cleaning and displays the first few rows of the DataFrame.
It calculates descriptive statistics for the data (mean, standard deviation, etc.).
Correlation and covariance matrices are generated to explore relationships between features.
Dates are converted to datetime format for time series analysis.
A bar plot visualizes historical prices over dates.
A histogram and a line plot are created to further analyze the price distribution and trends.
Time Series Forecasting with SARIMA:

The code utilizes the statsmodels library for time series analysis.
It checks for stationarity of the data using the Augmented Dickey-Fuller test (not explicitly shown).
A SARIMA model is defined with specific parameters (order and seasonal order) to capture seasonality and trends in the data.
The model is fitted on the training data.
Future price values are forecasted for the test data.
The forecasted values, along with confidence intervals, are plotted against the actual test data to evaluate the model's performance.
Mean Squared Error (MSE) is calculated to quantify the forecasting accuracy.
Note:

This is a starting point, and the specific SARIMA parameters and model selection might require further optimization based on the data characteristics.
Additional features or considerations can be incorporated to enhance the model's accuracy, such as including relevant economic indicators or incorporating external factors impacting commodity prices.
Overall, this project showcases a data-driven approach to pricing a commodity storage contract by leveraging time series analysis techniques.
