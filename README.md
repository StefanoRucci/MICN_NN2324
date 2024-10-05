# Neural Network Project - Multi-Scale Isometric Convolution Network (MICN)
## Course: Neural Networks (2023/2024)

### Project Overview
This project is based on the implementation and evaluation of the **Multi-scale Isometric Convolution Network (MICN)**, a model presented in the scientific paper ["MICN: Multi-scale Local and Global Context Modeling for Long-term Series Forecasting"](https://github.com/wanghq21/MICN), published at ICLR 2023. The paper proposes a novel approach to time-series forecasting that balances computational efficiency and predictive accuracy by combining local features and global correlations through multi-scale convolutions.

### Objective
The objective of this project was to:
1. Model and preprocess the datasets to extract necessary features for training.
2. Implement the MICN model as described in the paper.
3. Compare the performance of the MICN model with traditional models such as **ARIMA**, **Support Vector Regression (SVR)**, **LSTM**, and **CNN**.
4. Analyze the strengths and weaknesses of each approach, including computational efficiency and forecasting accuracy.

### Datasets and Preprocessing
The datasets used in this project come from various sources relevant to long-term time series forecasting (such as weather, traffic, and electricity consumption). Each dataset underwent extensive preprocessing to ensure suitability for model training. The key preprocessing steps included:
- **Feature extraction**: Extracting relevant temporal and spatial features.
- **Data normalization**: Normalizing the data for stable and efficient model training.
- **Handling missing values**: Imputing or discarding missing data points to maintain data integrity.

### MICN Model Implementation
The core of the project is the implementation of the **Multi-scale Isometric Convolution Network (MICN)**, which integrates both local and global patterns using multi-scale convolutions:
- **Local features** are captured via down-sampled convolutions.
- **Global correlations** are modeled through isometric convolutions, enabling the model to understand long-term dependencies in the time series data.
The model was implemented following the architecture outlined in the original paper, with hyperparameters tuned to optimize performance on the dataset.

### Other Models Implemented
In addition to MICN, several other traditional models were implemented and evaluated for comparison:
- **ARIMA (Auto-Regressive Integrated Moving Average)**: A classic statistical method for time series forecasting.
- **Support Vector Regression (SVR)**: A machine learning regression model.
- **LSTM (Long Short-Term Memory)**: A type of recurrent neural network (RNN) well-suited for sequential data.
- **CNN (Convolutional Neural Network)**: Adapted for time-series forecasting using 1D convolutions to extract features.

### Model Comparison
The performance of MICN was compared with ARIMA, SVR, LSTM, and CNN models based on forecasting accuracy (using metrics such as Mean Absolute Error (MAE) and Mean Squared Error (MSE)) and computational efficiency. The comparison focused on:
- **Accuracy**: How well the models performed in capturing both short-term fluctuations and long-term trends.
- **Efficiency**: Computational time and resource usage for each model.

### Results
- **MICN** demonstrated significant improvements in forecasting accuracy compared to ARIMA and SVR models, particularly in capturing both short-term and long-term patterns.
- **LSTM** and **CNN** models also showed good performance but had limitations in handling longer-term dependencies efficiently.
- **ARIMA** and **SVR** performed reasonably well for short-term forecasts but struggled with scalability and accuracy over longer time periods.

### Conclusions
This project highlights the effectiveness of the **MICN** model for long-term time series forecasting. Its ability to balance local feature extraction and global pattern recognition while maintaining computational efficiency makes it a promising solution for various real-world forecasting tasks.

### How to Run
1. Clone this repository: 
   ```bash
   git clone <repository-url>
   cd <repository-folder>
