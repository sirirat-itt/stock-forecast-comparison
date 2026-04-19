## Stock Price Forecasting — Model Comparison (LSTM vs CNN vs ARIMA vs ANN)
> Senior Project | Faculty of Science, Department of Statistics, Kasetsart University | 2022–2025

## Objective
To compare the forecasting performance of four machine learning and statistical models — **ARIMA**, **LSTM**, **ANN**, and **CNN** — on international and Thai stock market data, and identify the most suitable model for each asset type.

## Stocks & Data

| Stock | Description | Market |
|-------|-------------|--------|
| VIX | CBOE Volatility Index | US |
| MSFT | Microsoft Corporation | US (NASDAQ) |
| TSLA | Tesla, Inc. | US (NASDAQ) |
| AOT | Airports of Thailand PCL | Thailand (SET) |

- **Period:** January 2022 – August 2025
- **Frequency:** Daily closing price
- **Source:** [Investing.com](https://www.investing.com)

## Models Compared

| Model | Type | Library |
|-------|------|---------|
| ARIMA | Statistical Time Series | statsmodels |
| LSTM | Recurrent Neural Network | TensorFlow / Keras |
| ANN | Feedforward Neural Network | TensorFlow / Keras |
| CNN | Convolutional Neural Network | TensorFlow / Keras |

## Results — MAPE (%) on Test Set

Lower is better ↓

| Stock | Best Model | MAPE (%) |
|-------|-----------|----------|
| MSFT | LSTM | **1.21%** |
| TSLA | LSTM | **3.30%** |
| VIX | LSTM | **6.56%** |
| AOT | CNN | **2.91%** |

**Key Findings:**
- LSTM outperformed other models on US stocks (MSFT, TSLA, VIX), achieving the lowest MAPE of **1.21%** on MSFT
- CNN performed best on Thai stock AOT with a MAPE of **2.91%**
- Deep learning models (LSTM, CNN) consistently outperformed traditional ARIMA on all assets

## Tools & Technologies

- **Language:** Python 3.x
- **Libraries:** TensorFlow, Keras, statsmodels, pandas, numpy, matplotlib, scikit-learn
- **Evaluation Metric:** MAPE (Mean Absolute Percentage Error)
- **Environment:** Google Colab / Jupyter Notebook
## Repository Structure
stock-forecast-comparison/
├── Project_AOT.ipynb          ← CNN model (AOT)
├── Project_Microsoft.ipynb    ← LSTM model (MSFT)
├── Project_Tesla.ipynb        ← LSTM model (TSLA)
├── Project_VIXipynb.ipynb     ← LSTM model (VIX)
├── Airports of Thailand Stock Price History.csv
├── CBOE Volatility Index Historical Data.csv
├── Microsoft Stock Price History.csv
├── Tesla Stock Price History.csv
└── README.md
## How to Run
1. Clone this repository
2. Open any `.ipynb` file in Google Colab or Jupyter Notebook
3. Upload the corresponding CSV file
4. Run all cells

| Notebook | Stock | Best Model |
|----------|-------|-----------|
| Project_AOT.ipynb | AOT | CNN |
| Project_Microsoft.ipynb | MSFT | LSTM |
| Project_Tesla.ipynb | TSLA | LSTM |
| Project_VIXipynb.ipynb | VIX | LSTM |

## Author
**Sirirat Ittisuriyakun**  
B.Sc. Statistics — Kasetsart University  
📧 sirirat.it@ku.th
