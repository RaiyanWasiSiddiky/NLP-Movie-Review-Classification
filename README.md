# Movie Review Classifier - NLP Project

## Team Information

| Name                |
|---------------------|
| Shihab Muhtasim  |
| Raiyan Wasi Siddiky |

## Introduction

This project, titled "Movie Review Classifier," delves into Natural Language Processing (NLP) to create a sentiment analysis algorithm for movie reviews. The classification task involves training models on a dataset of movie reviews and categorizing them as either positive or negative. The project explores three different models: a shallow neural network, an LSTM model, and a bidirectional LSTM model.

## Instructions 

As the project was executed on Google Colab, it is recommended to run the code on the same platform due to potential compatibility issues with local IDEs. Instructions for uploading necessary files are provided in the code. The required files are `imdb_440.zip` (IMDB dataset file) and `glove.6B.100d.txt` (GloVe embeddings file).

## Coding Tasks

### 1. Loading the Dataset
- Utilized Pandas to read the CSV file containing movie reviews and their classifications.
- Checked dataset characteristics, ensuring a balanced sentiment distribution.

### 2. Converting Reviews into Vectors
- Tokenized reviews using Keras' Tokenizer module.
- Employed pre-trained GloVe word embeddings to convert reviews into fixed-length vectors.

### 3. Splitting the Dataset
- Used `train_test_split` from `sklearn.model_selection` for an 80-20 split between training and testing data.

### 4. Training the Shallow Model
- Implemented a neural network with an embedding layer, dense layer, and output layer.
- Utilized pre-trained GloVe weights.
- Trained for 20 epochs, experimenting with hyperparameters.

### 5. LSTM
a. **Unidirectional LSTM**
   - Replaced the second layer with a unidirectional LSTM layer.
   - Maintained the same batch size, optimizer, and loss functions.

b. **Bidirectional LSTM**
   - Introduced bidirectional information flow with a bidirectional LSTM layer.
   - Maintained a similar architecture to the unidirectional LSTM model.

### 6. Analysis
- Compared performance metrics of the three models.
- Noted overfitting in the shallow model, balanced bias-variance trade-off in the unidirectional LSTM model, and slight overfitting in the bidirectional LSTM model.
- Discussed potential improvements, including regularization techniques, dropout, pooling layers, and advanced models like transformers or GRUs.
  

### Suggestions for Improvement
- Introduced regularization techniques, such as lasso or ridge regression.
- Discussed the potential use of dropout, pooling layers, early stopping, attention mechanisms, and advanced models like transformers or GRUs.
- Mentioned experimentation with different hyperparameter configurations for optimization.
