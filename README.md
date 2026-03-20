# 🔌 Appliance Energy Consumption Prediction  
### Multivariate Time-Series Forecasting using Machine Learning & Deep Learning

---

## 📌 Project Overview

This project focuses on predicting **appliance energy consumption** using a multivariate time-series dataset containing environmental, temporal, and sensor-based features recorded at 10-minute intervals.

The goal is to build accurate predictive models by applying:
- Data preprocessing
- Feature engineering
- Machine learning and deep learning techniques

Both **baseline (Linear Regression)** and **deep learning models (LSTM, GRU, CNN-LSTM)** are implemented and compared.

---

## 🎯 Objectives

- Analyze and preprocess time-series data
- Engineer meaningful temporal and statistical features
- Develop and evaluate predictive models
- Compare baseline and deep learning approaches
- Optimize model performance

---

## 📂 Project Structure 
├── data/
│   ├── raw/                # Original dataset
│   
│
├── notebooks/
│   └── EDA.ipynb           # Exploratory Data Analysis (EDA)
│
├── src/
│   ├── data_preprocessing.py   # Data cleaning and preprocessing scripts
│   ├── feature_engineering.py  # Feature creation and transformation logic
│   ├── model.py                # Deep learning model definitions (LSTM, GRU, CNN-LSTM)
│   └── train.py                # Model training pipeline
│
├── models/
│   └── trained_model.h5    # Saved trained model
│
├── reports/
│   └── report.pdf          # Final project report
│
├── requirements.txt        # Project dependencies
│
└── README.md               # Project documentation

