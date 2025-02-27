# Omdena_Workshop_Time_Series_Webinar



# Amazon Stock Price Time Series Analysis

This project performs a time series analysis on Amazon (AMZN) stock prices using Python libraries such as `yfinance` for data retrieval and `prophet` for forecasting. The notebook downloads historical stock data, processes it, and provides visualizations of trends and seasonal components.

## Prerequisites

To run this notebook, you need to install the required Python packages. The following command installs them:

```bash
pip install prophet yfinance

Required Libraries

pandas: Data manipulation and analysis
numpy: Numerical computations
matplotlib.pyplot: Plotting visualizations
statsmodels: Statistical modeling and time series analysis
yfinance: Fetching stock data from Yahoo Finance
prophet: Time series forecasting (installed via pip)
Data
The notebook retrieves historical stock price data for Amazon (AMZN) from Yahoo Finance using the yfinance library.

Data Details

Ticker: AMZN
Start Date: January 1, 2023
End Date: January 31, 2024
Columns: Open, High, Low, Close, Adjusted Close, Volume
Sample Data

Here’s a preview of the first few rows of the downloaded data:

Date	Open	High	Low	Close	Adj Close	Volume
2023-01-03	85.459999	86.959999	84.209999	85.820000	85.820000	76706000
2023-01-04	86.550003	86.980003	83.360001	85.139999	85.139999	68885100
2023-01-05	85.330002	85.419998	83.070000	83.120003	83.120003	67930800
2023-01-06	83.029999	86.400002	81.430000	86.080002	86.080002	83303400
2023-01-09	87.459999	89.480003	87.080002	87.360001	87.360001	65266100



Code Overview
1. Install Dependencies

The notebook starts by installing prophet and yfinance:

!pip install prophet yfinance


Usage
Clone this repository or download the notebook.
Install dependencies by running the pip install command above in your environment.
Run the notebook in a Jupyter environment (e.g., Google Colab, Jupyter Notebook) to fetch the data and generate visualizations.
Modify the symbol, start, or end variables to analyze different stocks or date ranges.

Notes
The notebook assumes an internet connection to fetch data from Yahoo Finance.
The prophet library is used for forecasting, but the specific model training and forecasting steps are not shown in the provided snippet. Ensure these steps are completed before calling plot_components_plotly.
The visualizations are rendered using Plotly, which provides interactive plots.

License
This project is unlicensed and provided as-is for educational purposes.
