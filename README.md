# Time Series Forecasting for Ambulance Call Volumes

Forecasting daily emergency ambulance call volumes using classical time series models in Python, with the goal of supporting staffing and resource allocation planning.

---

## Project Overview

This project analyses ambulance service call data from Jakarta, Indonesia (March 2019 – September 2019) to predict future daily emergency demand. By identifying underlying seasonal patterns and benchmarking multiple forecasting models, the project produces a 60-day forward forecast to aid operational planning.

---

## Key Findings

- A clear **7-day seasonality** was identified through seasonal decomposition and ACF/PACF analysis
- **SARIMA** outperformed all other models, capturing the weekly seasonal component most effectively
- A **60-day forecast** was generated to support ambulance staffing and resource planning decisions

---

## Models Benchmarked

| Model | Notes |
|---|---|
| Naive | Baseline comparison |
| Simple Exponential Smoothing (SES) | Weighted recent observations |
| Holt-Winters | Captures trend + seasonality |
| ARIMA | Non-seasonal autoregressive model |
| **SARIMA** | **Best performer — seasonal ARIMA** |

Models were evaluated using an **80/20 train-test split** with MAE and RMSE as performance metrics.

---

## Project Structure

```
├── timeseries.ipynb   # Full analysis and modelling notebook
├── Time Series Poster.pdf       # Visual summary of methodology and results
└── README.md
```



## Tools & Libraries

- **Python** — Pandas, NumPy, Matplotlib
- **statsmodels** — ARIMA, SARIMA, Holt-Winters, seasonal decomposition
- **Jupyter Notebook**

---

## Dataset

Ambulance emergency call data from Jakarta, Indonesia covering March 2019 – September 2019. Raw data consists of timestamped call records which were aggregated into daily counts for modelling.

---

## Author

**Rutvik Randive**  
