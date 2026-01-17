# Time Series Project

This repository contains a sequence of Jupyter notebooks and datasets exploring time series analysis and forecasting using practical, hands-on examples. Notebooks progress from data cleaning to ARIMA+GARCH modeling and forecasting, using Python data tools and statistical libraries.

## Data Cleaning

This section demonstrates ingesting and preparing monthly time series data (CSV) for analysis: parsing dates, handling missing values, smoothing, and resampling. Implementations use `pandas` and `numpy` for transformations, and `matplotlib`/`seaborn` for visual checks and exploratory plots.

## Basic Time Series Analysis

Explores seasonality, trends, decomposition, autocorrelation, and stationarity diagnostics. Visual and statistical techniques (ACF/PACF, rolling statistics) are applied using `statsmodels`, `pandas`, and plotting libraries to motivate appropriate modeling choices and parameter selection.

## ARIMA Modeling

Builds, validates, and tunes ARIMA/SARIMA models for the prepared series, including differencing, order selection (ACF/PACF, information criteria), residual checks, and performance reporting. For series with time-varying volatility (e.g., financial , economic variable data), also fit ARCH/GARCH models to capture conditional heteroskedasticity using `arch` or `statsmodels`.

## Forecasting

Uses fitted models to generate out-of-sample forecasts with confidence intervals, visual comparisons to actuals, and basic error metrics (MAE, RMSE). Forecast workflows combine model outputs with `pandas` time indexing and `matplotlib`/`seaborn` visualization for presentation.

## Example Notebook

Provides a concise end-to-end demonstration of the workflow on a sample dataset: data load, quick cleaning, ARIMA fit, and short-term forecast. This notebook shows reproducible commands you can adapt to your own CSV time series files.

## Data

Included CSVs (`cpi_month.csv`, `Europe_Brent_Spot_Price_FOB.csv`) are example monthly series used throughout the notebooks. Each file is read with `pandas` and serves to illustrate preprocessing, decomposition, and forecasting pipelines.

## Requirements

- Python 3.8+ (recommended)
- Jupyter Notebook / JupyterLab
- pandas, numpy
- matplotlib, seaborn
- statsmodels
- scikit-learn (for preprocessing helpers, optional)
- pmdarima (optional, for automated ARIMA selection)

Install with:

```
pip install -r requirements.txt
```

or individually, e.g. `pip install pandas numpy matplotlib seaborn statsmodels pmdarima jupyter`.

## Run

Open the notebooks in Jupyter and run cells in order: `1_data_cleaning.ipynb`, `2_basic_timesereis.ipynb`, `3_ARIMA.ipynb`, `4_Forecasting.ipynb`. Modify dataset paths as needed and re-run to reproduce analyses and forecasts.
# time_series_project
Time series project for Crude Oil Prices and CPI of India and Brazil
