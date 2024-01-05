
# NOK to USD Price Prediction Using LSTM Neural Network

## Overview
This project aims to predict the exchange rate between the Norwegian Krone (NOK) and the American Dollar (USD) using a Long Short-Term Memory (LSTM) neural network. This type of recurrent neural network is ideal for analyzing and forecasting currency exchange rates based on historical data.

## Disclaimer
Predictions from this LSTM model should not be used as the sole basis for financial decisions. Financial markets are complex and affected by many unpredictable factors. We highly recommend consulting with an economic specialist or financial advisor for in-depth analysis and professional advice.

## Installation
To set up this project, install the following Python libraries using pip:

```bash
pip install numpy pandas datetime tensorflow yahoo_fin sklearn matplotlib
```

## Data Description
The dataset for this project is sourced from Yahoo Finance, using the `yahoo_fin` library. It provides historical exchange rate data between the Norwegian Krone (NOK) and the American Dollar (USD). This data includes daily open, high, low, and close prices, which are essential for training and validating the LSTM model.

## Key Components
- **Import Libraries**: Includes libraries for data manipulation, model building, and visualization.
- **Configuration Settings**: Setup for window size (`N_STEPS`), lookup steps (`LOOKUP_STEPS`), and stock ticker symbol (`STOCK`).
- **Data Loading and Preprocessing**: Historical data loading for the past three years and preprocessing for the LSTM model.
- **LSTM Model Building**: Construction of a sequential LSTM model for time series prediction.
- **Training and Predictions**: Model training on historical data and future price predictions.
- **Visualization**: Plotting actual vs. predicted prices for model performance analysis.

## Model Architecture
The core of this project is the LSTM neural network model. LSTM, or Long Short-Term Memory, is a type of recurrent neural network (RNN) architecture that is well-suited for time series prediction tasks. It overcomes the limitations of traditional RNNs by effectively capturing long-term dependencies in data sequences, making it ideal for predicting financial market trends which involve complex, time-dependent patterns.

Key features of the LSTM model used in this project include:
- **Sequential Layer Structure**: The model is built using sequential layers, which allows for a straightforward stacking of LSTM and other layers.
- **LSTM Layers**: The model incorporates LSTM layers with a specified number of neurons. These layers are responsible for learning the temporal dependencies in the exchange rate data.
- **Dropout Layers**: To prevent overfitting, dropout layers are included, which randomly drop a set percentage of neurons during training.
- **Dense Layers**: After LSTM layers, dense layers are added to interpret the features learned by the LSTM layers and make the final prediction.

For a deeper understanding of LSTM networks and their applications, you can refer to the following resources:
- [Understanding LSTM Networks by Christopher Olah](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)
- [LSTM Neural Network for Time Series Prediction by Jakob Aungiers](https://www.jakob-aungiers.com/articles/a/LSTM-Neural-Network-for-Time-Series-Prediction)
- [TensorFlow LSTM API Documentation](https://www.tensorflow.org/api_docs/python/tf/keras/layers/LSTM)

## Contributing
Contributions to this project are welcome and free. Feel free to fork the repository and submit pull requests. If you have any questions or suggestions, you can reach out by emailing [farhad.vadiee@gmail.com](mailto:farhad.vadiee@gmail.com).

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
