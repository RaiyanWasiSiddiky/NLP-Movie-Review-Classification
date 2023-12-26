# NLP-Movie-Review-Classification
![GitHub top language](https://img.shields.io/github/languages/top/shihabmuhtasim/NLP-Movie-Review-Classification?color=f5f5dc)
![GitHub language count](https://img.shields.io/github/languages/count/shihabmuhtasim/NLP-Movie-Review-Classification?color=f5f5dc)
![GitHub last commit](https://img.shields.io/github/last-commit/shihabmuhtasim/NLP-Movie-Review-Classification?color=f5f5dc)
![GitHub repo file count](https://img.shields.io/github/directory-file-count/shihabmuhtasim/NLP-Movie-Review-Classification?color=f5f5dc)
![GitHub repo size](https://img.shields.io/github/repo-size/shihabmuhtasim/NLP-Movie-Review-Classification?color=f5f5dc)
![GitHub watchers](https://img.shields.io/github/watchers/shihabmuhtasim/NLP-Movie-Review-Classification?style=social)



## Introduction

This project, titled "Movie Review Classifier," delves into Natural Language Processing (NLP) to create a sentiment analysis algorithm for movie reviews. The classification task involves training models on a dataset of movie reviews and categorizing them as either positive or negative. The project explores three different models: a shallow neural network, an LSTM model, and a bidirectional LSTM model.
![15](https://github.com/shihabmuhtasim/NLP-Movie-Review-Classification/assets/92597456/d14e4038-048c-4f52-b388-a7ed5ce59a63)

## Team Information

| Name                |
|---------------------|
| Shihab Muhtasim  |
| Raiyan Wasi Siddiky |

## Datasets
- [Glov file](https://drive.google.com/file/d/1CLrwskD-M8ce0M5agxRjB3OhKuKiCcCn/view)
- [IMDB dataset](https://drive.google.com/file/d/1hyn6U44cvUNedMnzPHzHsiBgXMHFBjBw/view)

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
