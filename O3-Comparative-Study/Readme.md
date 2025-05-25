# Assessing Dataset Reliability for Ozone Level Prediction: A Comparative Study of ML and DL Approaches

## Abstract

Ground-level ozone (O₃) is a significant air pollutant with detrimental impacts on both the environment and human health. The Environmental Protection Agency (EPA) has defined six categories to classify ozone levels. This study aims to perform multi-class classification of ozone levels using both machine learning and deep learning models.

The dataset used includes various air quality indicators such as **PM10**, **NO2**, **SO2**, **O3**, **AQI**, **PM2.5**, and meteorological features like **temperature**, **humidity**, and **wind speed**. A new feature called **Ozone Category** was engineered using O₃ concentration levels based on EPA-defined thresholds.

To mitigate the issue of class imbalance, manual oversampling was conducted by duplicating instances from underrepresented categories. The models implemented in this study include:

- **Machine Learning**: Decision Trees, Random Forests, K-Nearest Neighbors (KNN)
- **Deep Learning**: Multi-Layer Perceptron (MLP), Convolutional Neural Network (CNN)
- **Recurrent Neural Networks**: Long Short-Term Memory (LSTM) and Bi-Directional LSTM (Bi-LSTM)

The models were evaluated using standard performance metrics such as **accuracy**, **precision**, **recall**, **F1-score**, and **ROC curves**.

This comparative analysis helps in identifying the most effective model for classifying ground-level ozone into EPA-defined categories, contributing to improved air quality monitoring and public health decision-making.

## Introduction

Ozone (O₃) is a triatomic molecule of oxygen, distinct from the more common diatomic form (O₂) that we breathe. While stratospheric ozone is essential for blocking the sun’s harmful ultraviolet (UV) rays, **ground-level ozone** is a major air pollutant. It adversely affects materials, vegetation, and human health.

Ground-level ozone is formed through complex **photochemical reactions** between nitrogen oxides (NOₓ) and volatile organic compounds (VOCs) in the presence of sunlight. These precursor emissions mainly originate from **anthropogenic sources** such as industrial activities, vehicle exhaust, and the use of certain solvents.

Accurate prediction and classification of ozone levels is critical, as **elevated concentrations can lead to respiratory illnesses** like asthma, bronchitis, and emphysema, especially in vulnerable populations such as children, the elderly, and individuals with pre-existing conditions. Ozone exposure can also **damage crops and forests**, lowering agricultural productivity and affecting ecosystem balance. The **economic consequences** of unmitigated ozone pollution include increased healthcare costs, loss of work productivity, and environmental degradation.

Traditional methods for predicting ozone levels often struggle to capture the **non-linear, multivariate interactions** between ozone, its chemical precursors, and meteorological factors such as temperature, humidity, and wind.

This study overcomes such limitations by leveraging a combination of **machine learning and deep learning techniques**, including:

- **Machine Learning**: K-Nearest Neighbors (KNN), Decision Tree (DT), Random Forest
- **Deep Learning**: Multi-Layer Perceptron (MLP), Convolutional Neural Network (CNN)
- **Recurrent Neural Networks**: Long Short-Term Memory (LSTM), Bidirectional LSTM (Bi-LSTM)
- **Proposed Hybrid Model**: An integrated architecture combining CNN, Vision Transformers (ViT), and Attention layers for improved performance

The performance of all models is evaluated based on **classification accuracy**, **generalization ability**, and standard metrics such as **precision**, **recall**, **F1-score**, and **ROC-AUC**. This study aims to enhance ground-level ozone classification to support **air quality management**, **health advisory systems**, and **policy formulation**.
