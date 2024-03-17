# Project: Multimodal Emotion Prediction under Stress (MuSe-Stress)

## Introduction

The Multimodal Sentiment Analysis (MuSe) 2021 challenge focuses on estimating emotion and sentiment through various sub-tasks, incorporating audio-visual, language, and biological signal modalities. One of these sub-challenges, MuSe-Stress, specifically targets continuous emotion prediction under stressful conditions. This report details the methodologies, analyses, and outcomes of addressing the MuSe-Stress challenge.

**Guided by Prof'in Hanna Drimalla and Herr Matthias Norden**

## Project Overview

### Objective

The primary goal of this project is to develop effective models for predicting continuous emotional states (valence and arousal) using the Ulm-TSST database, a collection of recordings obtained from individuals undergoing stress-inducing tasks.

### Methodology

1. **Baseline Model Setup:**
   - Implement a baseline Long Short-Term Memory (LSTM) model, considering its capability in handling sequential data.
   - Explore different configurations, such as varying hidden layer dimensions and learning rates, to optimize model performance.
   - Utilize a windowing method to segment input features during training.

2. **Feature Selection and Engineering:**
   - Investigate feature sets (e.g., egemaps, VGGface) to identify those exhibiting strong correlations with valence and arousal.
   - Employ correlation analysis to filter features and select the most relevant ones for stress prediction.
   - Extract and preprocess features from the Ulm-TSST database, including acoustic, visual, and psychological signals.

3. **Model Comparison:**
   - Compare the baseline LSTM model with alternative architectures, such as Convolutional Neural Networks (CNN) and Gated Recurrent Units (GRU), to assess their effectiveness in stress prediction.
   - Evaluate model performance using appropriate metrics, including mean squared error and concordance correlation coefficient.

4. **Late Fusion Technique:**
   - Apply late fusion to combine predictions from multiple modalities (e.g., audio, video, psychological signals) to enhance overall performance.

## Data Exploration

- Conduct exploratory data analysis to understand the relationships between different features and the target emotional states (valence and arousal).
- Utilize correlation matrices and heatmaps to visualize feature dependencies and identify significant correlations.

## Training Models

### LSTM Baseline Model

- Configure the LSTM model architecture with multiple layers to capture sequential dependencies in the input features.
- Experiment with different hyperparameters, such as learning rate and hidden layer dimensions, to optimize model performance.
- Employ windowing techniques to segment input features and labels during training.

### CNN Model for Image Data

- Train a CNN model using raw images extracted from the Ulm-TSST database to predict valence and arousal.
- Preprocess raw images and ensure compatibility with the CNN input layer.
- Evaluate model performance using the concordance correlation coefficient.

## Evaluation and Results

- Assess model performance using appropriate evaluation metrics, such as mean squared error and concordance correlation coefficient.
- Compare the performance of different models and architectures to identify the most effective approach for stress prediction.
- Discuss the implications of the findings and potential areas for future research and improvement.

## Conclusion

The project aims to develop robust models for continuous emotion prediction under stress conditions using multimodal data sources. By exploring various architectures, feature engineering techniques, and evaluation metrics, the goal is to advance the state-of-the-art in affective computing and contribute to applications such as stress detection and emotion-aware systems.
