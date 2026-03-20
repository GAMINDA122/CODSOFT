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
## 📁 Project Structure

```bash
├── data/
│   ├── raw/                # Original dataset
│   └── processed/          # Cleaned/processed data
├── notebooks/
│   └── EDA.ipynb           # Exploratory Data Analysis
├── src/
│   ├── data_preprocessing.py
│   ├── feature_engineering.py
│   ├── model.py
│   └── train.py
├── models/
│   └── trained_model.h5    # Saved trained model
├── reports/
│   └── report.pdf          # Final report
├── requirements.txt
└── README.md
```
---

## ⚙️ Technologies Used

- **Python 3.x**
- **Pandas, NumPy** → Data manipulation
- **Matplotlib, Seaborn** → Visualization
- **Scikit-learn** → Machine learning models
- **TensorFlow / Keras** → Deep learning models

---

## 📊 Dataset Description

- ~20,000 records
- 10-minute interval time-series data
- Features include:
  - Temperature (T1–T6)
  - Humidity (RH_1–RH_6)
  - Weather conditions
  - Time-based features
  - Target: **Appliances (energy consumption in Wh)**

---

## 🔄 Workflow

### 1. Data Preprocessing
- Missing value handling (interpolation)
- Outlier detection (IQR method)
- Data scaling (MinMaxScaler)
- Time-based train-test split

### 2. Feature Engineering
- Time-based features (hour, day, month)
- Lag features (lag_1, lag_3, lag_6)
- Rolling statistics (mean, std)
- Interaction features
- Feature selection (RFE, Random Forest)

### 3. Model Development
- Baseline: Linear Regression
- Deep Learning:
  - LSTM
  - GRU
  - CNN-LSTM

### 4. Evaluation Metrics
- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R² Score
- MAPE

### 5. Model Optimization
- Hyperparameter tuning
- Dropout regularization
- Early stopping
- Learning rate scheduling

--- 
## 📈 Key Results

| Model                 | RMSE  | R²   |
|----------------------|-------|------|
| Linear Regression    | 13.79 | 0.67 |
| CNN-LSTM (Optimized) | 17.17 | 0.49 |

### 🏆 Final Insight:
> Linear Regression outperformed deep learning models due to strong feature engineering and structured data representation.
---

## 🚀 Installation & Setup

### 1. Clone the Repository
```bash

```
### 2. Create Virtual Environment (Recommended) 
```bash
python -m venv env
source env/bin/activate   # Linux / Mac
env\Scripts\activate      # Windows
```
### 2. Create Virtual Environment (Recommended) 
```bash
pip install -r requirements.txt
```

## ▶️ How to Run the Project

### Option 1: Run Notebook

- Open **Jupyter Notebook** or **Google Colab**

- Run the following file:

```bash
notebooks/EDA.ipynb
```
## 💾 Model Saving

Trained model is saved at:

```bash
models/trained_model.h5
```

### Load Model

```python
from tensorflow.keras.models import load_model
model = load_model("models/trained_model.h5")
```

---

## 📄 Report

Detailed explanation is available in:

```bash
reports/report.pdf
```

### Includes:

- EDA insights  
- Model design  
- Evaluation results  
- Optimization analysis 


## 📌 Key Learnings

- Feature engineering is critical in time-series modeling  
- Deep learning is not always superior  
- Simpler models can outperform complex ones when data is well-prepared  
- Model selection must be based on data characteristics  

---

## 🔮 Future Improvements

- Use larger datasets  
- Apply advanced models (XGBoost, LightGBM)  
- Implement pure sequence-based deep learning models  
- Use Bayesian hyperparameter optimization  
- Incorporate external data (weather, holidays)  

---

## 👤 Author

**A.M. Gaminda Premasiri**  
Undergraduate – University of Kelaniya  
AI/ML Enthusiast  

---

## 📜 License

This project is for educational and research purposes.



               
               



















  
