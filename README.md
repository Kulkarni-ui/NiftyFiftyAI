# NiftyFiftyAI

# 📈 AI for Banking and Finance — Nifty 50 Index Tracking using ML & DL

A project that leverages **Machine Learning** and **Deep Learning** to replicate the performance of the **Nifty 50 Index**, minimizing tracking error with traditional regressions and neural network models.

---

## 🔍 Objective

To construct a **model-based portfolio** that closely mimics the **Nifty 50 Index** by minimizing **Tracking Error (TE)** using:

- 🔹 **Traditional ML Models**: Ridge, Lasso, and ElasticNet
- 🔹 **Deep Learning Model**: Autoencoder

---

## 📘 Introduction

**Index tracking** is central to passive investing and ETF management. This project demonstrates how **AI techniques** can be employed to build a portfolio that tracks the **Nifty 50 Index** using historical price data.

We:
- Fetch and preprocess data from 2018–2024
- Train models to learn relationships between constituent stock returns and the index
- Evaluate model performance with metrics and plots
- Compare traditional and deep learning approaches

---

## 🛠️ Tools & Technologies

- **Language**: Python 3.x  
- **Data Source**: [`yfinance`](https://pypi.org/project/yfinance/)
- **Libraries**:
  - Data Handling: `pandas`, `numpy`
  - Modeling: `scikit-learn`, `tensorflow`, `keras`
  - Visualization: `matplotlib`, `seaborn`

---

## 📊 Dataset Overview

| Feature       | Description                           |
|--------------|---------------------------------------|
| **Source**    | Fetched using `yfinance` API          |
| **Index**     | Nifty 50 (^NSEI)                      |
| **Assets**    | 50 constituent stocks                 |
| **Period**    | 01-Jan-2018 to 31-Dec-2024            |
| **Frequency** | Daily closing prices                  |

---

## 🔁 Project Workflow

### 1. 🧠 Data Collection
- Download historical prices for index and stocks

### 2. 🔧 Feature Engineering
- Compute **log returns** for stationarity
- Prepare stock returns as features, index returns as target

### 3. 🧪 Train-Test Split
- **Train**: 2018–2021  
- **Test**: 2022–2024

### 4. ⚙️ Modeling
- Ridge, Lasso, ElasticNet with time-series CV
- Autoencoder for latent feature extraction and reconstruction

### 5. 📏 Evaluation Metrics
- **Tracking Error (TE)**: How closely model tracks index  
- **R² Score**: Variance explained  
- **Mean Squared Error (MSE)**: Accuracy of predictions

---

## 📈 Results

- 🔸 **Ridge and Lasso** showed strong generalization and low tracking error.
- 🔸 **Autoencoder** captured non-linear patterns and delivered competitive results.
- 🔸 Rolling TE and cumulative returns show the model’s portfolio tracking the index effectively.

---

## ✅ Conclusion

This project illustrates how **AI can enhance financial strategies** by accurately tracking indices like Nifty 50 using a hybrid of regression and neural network models.  
It provides a **foundation for ETF construction** and **passive investment modeling** in real-world financial systems.

---

## 🚀 Future Improvements

- 📉 Add **dynamic portfolio rebalancing**
- 📈 Explore **LSTM or transformer models** for temporal data
- 💸 Integrate **transaction costs and risk measures**
- 🔄 Use **real-time data streaming and model updating**

---

## 📂 Repository Structure

```
.
├── data/                   # Processed or raw data files
├── models/                 # Trained models (ML & DL)
├── notebooks/              # Jupyter/Colab notebooks
├── utils/                  # Utility scripts
├── main.py                 # Main pipeline
└── README.md               # Project overview
```

---

## 🙌 Acknowledgments
- Inspired by applications of AI in **Quantitative Finance**
