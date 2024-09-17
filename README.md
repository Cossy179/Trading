
# Bitcoin Price Prediction

## Overview

This project aims to predict Bitcoin prices using a Long Short-Term Memory (LSTM) neural network. It involves collecting historical Bitcoin price data from Binance, preprocessing the data, and training a machine learning model to forecast future prices.

## Project Structure

- **BTC Price predict.ipynb**: A Jupyter notebook that sets up the environment, preprocesses data, and implements an LSTM model to predict Bitcoin prices.
- **BTC puller.ipynb**: A Jupyter notebook dedicated to collecting Bitcoin price data using the Binance API via two methods: `ccxt` and direct HTTP requests.
- **BTC-USD.csv**: A CSV file containing historical hourly Bitcoin trading data, including Open, High, Low, Close prices, and Volume.

## Installation

1. Clone the repository.
2. Install the required Python libraries:

   ```bash
   pip install tensorflow pandas numpy matplotlib scikit-learn keras ccxt requests
   ```

3. Ensure you have access to the Binance API if fetching new data.

## Usage

1. **Data Collection**:
   - Use `BTC puller.ipynb` to fetch the latest Bitcoin price data and save it as a CSV file.
   
2. **Model Training**:
   - Open `BTC Price predict.ipynb` and run the cells to preprocess the data and train the LSTM model.
   - The notebook includes steps for scaling the data, splitting it into training and testing sets, and setting up the LSTM architecture.

3. **Prediction**:
   - After training, use the model to predict future Bitcoin prices and visualize the results.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the MIT License.
