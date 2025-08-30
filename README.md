This project implements a Bitcoin price prediction model using a Long Short-Term Memory (LSTM) neural network, built with TensorFlow and Keras. The model is designed to analyze historical time-series data and forecast future price movements.

## Project Structure
- **bitcoin-price-prediction.ipynb**: The main Jupyter Notebook containing the complete code for data preprocessing, model building, training, and prediction.  
- **BTC-USD.csv**: The dataset used for training and evaluating the model. It contains historical price data for Bitcoin.

## Dependencies
The project requires the following Python libraries. You can install them using pip:

```bash
pip install tensorflow keras pandas numpy scikit-learn matplotlib
How to Run
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
Ensure you have the data: Place the BTC-USD.csv file in the same directory as the Jupyter Notebook.

Launch Jupyter Notebook:

bash
Copy code
jupyter notebook
Open the bitcoin-price-prediction.ipynb file and run all the cells in sequence.

Methodology
The project follows these key steps:

Data Loading and Preprocessing:
The BTC-USD.csv file is loaded into a Pandas DataFrame.

The data is sorted by date.

The Close price is scaled using MinMaxScaler to normalize the values for the neural network.

The data is split into training and testing sets.

Model Architecture:
A Sequential model is built with the following layers:

Bidirectional LSTM: Highly effective for time-series data, as it processes the sequence both forwards and backwards.

Dropout: Used to prevent the model from overfitting.

Dense: The final output layer that provides the predicted price.

Training:
The model is compiled with the Adam optimizer and mean_squared_error as the loss function.

The model is trained on the preprocessed training data.

Prediction and Visualization:
The trained model makes predictions on the test set.

A custom function predicts future prices for a specified number of days.

The predictions are de-scaled to their original price values.

A plot is generated to visualize the actual prices, predicted prices, and the future forecast, providing a clear view of the model's performance.

Results
The visualization in the notebook shows the model's ability to track the actual Bitcoin price and its forecasted future trend.

Contributing
Feel free to open issues or submit pull requests to improve the model or add new features.
