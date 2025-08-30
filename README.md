# Bitcoin Price Prediction | LSTM

## Overview

This project focuses on forecasting Bitcoin prices using deep learning techniques. By training a Bidirectional Long Short-Term Memory (LSTM) model with TensorFlow and Keras, the system analyzes historical BTC-USD data and predicts future price movements. It includes end-to-end steps for preprocessing, model training, evaluation, and visualization.

## Features

✅ Bidirectional LSTM for robust sequence modeling of time-series data  
✅ MinMax scaling and sliding window generation for stable training  
✅ Dropout regularization to reduce overfitting  
✅ De-scaling of predictions back to original price units  
✅ Visualization of Actual vs. Predicted and multi-day Future Forecast

## Technologies Used

- **TensorFlow/Keras** – Model building and training  
- **Pandas/NumPy** – Data loading and manipulation  
- **scikit-learn** – MinMaxScaler and utilities  
- **Matplotlib** – Plotting and visualization

## Installation

### Prerequisites

Ensure you have Python installed (Python 3.8+ recommended). Install dependencies using:

```bash
pip install -r requirements.txt
```

### Clone the Repository

```bash
git clone https://github.com/Akashkittu/bitcoin_price_predictionn.git
cd bitcoin_price_prediction
```

## Dataset

- BTC-USD.csv containing historical Bitcoin prices (Date, Open, High, Low, Close, Adj Close, Volume).
- Place the file in the same directory as the notebook/script before running.

## Results

- Visualization of Actual vs. Predicted close prices on the test split.
- Future forecast overlay for a specified number of days.
- Error metrics (e.g., MSE/RMSE/MAE) can be reported from the notebook.

## Contributing

Feel free to fork this repository, create a branch, and submit a pull request for improvements
