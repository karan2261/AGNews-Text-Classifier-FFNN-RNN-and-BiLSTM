# AGNews-Text-Classifier-FFNN-RNN-and-BiLSTM
A text classification project using the AG News dataset, implementing and comparing three neural network architectures (FFNN, RNN, BiLSTM) with various optimizers.

## Overview
This project performs text classification on the AG News dataset using Feedforward Neural Networks (FFNN), Recurrent Neural Networks (RNN), and Bidirectional Long Short-Term Memory (BiLSTM) models. The dataset includes news articles categorized into four classes: World, Sports, Business, and Science/Technology.

## Features
- **Dataset**:
  - Training: 120,000 samples
  - Testing: 7,600 samples
- **Text Preprocessing**:
  - Cleaning and lemmatization using SpaCy.
  - Stopword removal using NLTK.
  - Tokenization and padding for sequence input.
- **Models**:
  - FFNN: Standard feedforward network with embedding and dense layers.
  - RNN: Simple Recurrent Neural Network for sequential text data.
  - BiLSTM: Bidirectional LSTM for capturing long-term dependencies.
- **Optimizers**:
  - Comparison using SGD, Adam, and Adagrad optimizers.
- **Evaluation Metrics**:
  - Accuracy and loss comparison across models and optimizers.

## Dataset
- **Source**: [AG News Corpus](https://labelbox.com/datasets/ag-news/)
- **Classes**:
  - World
  - Sports
  - Business
  - Science/Technology

## Workflow
1. **Text Preprocessing**:
   - Clean text data: Remove URLs, hashtags, punctuation, and extra spaces.
   - Tokenize and lemmatize text.
   - Remove stopwords from SpaCy and NLTK.
   - Visualize data distribution and most common words using word clouds and bar plots.
2. **Data Preparation**:
   - Tokenization and sequence padding.
   - Encode labels and split data into training and testing sets.
3. **Model Training**:
   - Train FFNN, RNN, and BiLSTM models using SGD, Adam, and Adagrad optimizers.
   - Use early stopping to prevent overfitting.
4. **Evaluation**:
   - Measure accuracy and loss.
   - Compare results across models and optimizers.
5. **Visualization**:
   - Generate plots for accuracy and loss comparisons.
  
## Results
- **Best Performing Model**: Bidirectional LSTM with Adagrad optimizer (Accuracy: 87.58%).

## Key Takeaways
- **Model Comparison**:
  - Bidirectional LSTM performed best among the models.
  - Optimizer choice significantly impacted model performance.
  - RNN struggled with vanishing gradients and achieved poor accuracy.
  - 
- **Preprocessing**:
  - Proper text cleaning and lemmatization improved model accuracy.
