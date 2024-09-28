# Neural Network Project - Multi-Scale Isometric Convolution Network (MICN)
## Course: Neural Networks (2023/2024)

### Project Overview
This project is based on the implementation and evaluation of the Multi-scale Isometric Convolution Network (MICN), a model presented in the scientific paper ["MICN: Multi-scale Local and Global Context Modeling for Long-term Series Forecasting"](https://github.com/wanghq21/MICN), which was published at ICLR 2023. The paper proposes a novel approach to time-series forecasting that balances computational efficiency and predictive accuracy by combining local features and global correlations through multi-scale convolutions.

### Objective
The objective of this project was to:
1. Model the datasets to extract and preprocess the necessary features for training.
2. Implement the MICN model as described in the paper.
3. Compare the performance of the MICN model with existing state-of-the-art models for long-term time series forecasting, analyzing the strengths and weaknesses of each approach.

### Datasets and Preprocessing
The datasets used in this project come from various sources relevant to long-term time series forecasting (such as weather data, traffic, and electricity consumption). Each dataset underwent extensive preprocessing to ensure that it was suitable for model training. The key preprocessing steps included:
- **Feature extraction**: Extracting key temporal and spatial features.
- **Data normalization**: Ensuring that the data were normalized for stable and efficient model training.
- **Handling missing values**: Imputing or discarding any missing data points to maintain the integrity of the dataset.

### MICN Model Implementation
The core of the project involved the implementation of the MICN model, which integrates both local and global patterns using multi-scale convolutions:
- **Local features** are captured via down-sampled convolutions.
- **Global correlations** are modeled through isometric convolutions to understand long-term dependencies in the time series data.
The model was implemented following the architecture outlined in the original paper, and various hyperparameters were tuned to optimize performance on the datasets.

### Model Comparison
To evaluate the performance of MICN, the following existing models were used for comparison:
- **Temporal Convolution Network (TCN)**: A CNN-based model for time series forecasting.
- **Transformer-based models** (such as Informer and Autoformer): Known for their effectiveness in modeling long-term dependencies but with higher computational complexity.
The comparison focused on accuracy, computational efficiency, and scalability.

### Results
- The MICN model demonstrated significant improvements in forecasting accuracy compared to the baseline models, particularly in capturing both short-term fluctuations and long-term trends.
- MICN outperformed other models in terms of computational efficiency, achieving linear time complexity with respect to the input sequence length.

### Conclusions
This project highlights the effectiveness of the MICN model for long-term time series forecasting. Its ability to balance local feature extraction and global pattern recognition, while maintaining computational efficiency, makes it a promising solution for a variety of real-world forecasting tasks.
