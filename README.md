# Time Series Analysis Workshop

This Jupyter notebook contains code and analysis from an Omdena workshop on Time Series forecasting.

## Key Components

- Stationarity Testing using Augmented Dickey-Fuller test
- Time series decomposition
- Statistical analysis
- Forecasting models

## Code Examples

The notebook includes utility functions like:

```python
def test_stationarity(data):
    result = adfuller(data)
    print('ADF Statistic: %f' % result[0])
    print('p-value: %f' % result[1])
    print('Critical Values:')
    for key, value in result[4].items():
        print(f'\t{key}: {value}')
    if result[1] < 0.05:
        print("Reject the null hypothesis. The data is stationary.")
    else:
        print("Fail to reject the null hypothesis. The data is non-stationary.")