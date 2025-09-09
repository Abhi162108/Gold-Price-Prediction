# 🏆 Gold Price Prediction  

This project predicts **Gold Prices (GLD)** using **financial indicators** such as the **S&P 500 Index (SPX), Oil Prices (USO), Silver Prices (SLV), and EUR/USD exchange rate**.  
The goal is to build a **machine learning model** that helps investors, analysts, and researchers forecast gold price trends.  

---

## 📊 Dataset  

The dataset contains daily market data:  

| Column    | Description |
|-----------|-------------|
| **Date**   | Trading date |
| **SPX**    | S&P 500 Index (US stock market benchmark) |
| **GLD**    | SPDR Gold Shares ETF (proxy for gold price) |
| **USO**    | United States Oil Fund (proxy for crude oil prices) |
| **SLV**    | iShares Silver Trust (proxy for silver prices) |
| **EUR/USD**| Euro to US Dollar exchange rate |

Example data:  

| Date     | SPX       | GLD   | USO   | SLV   | EUR/USD |
|----------|----------:|------:|------:|------:|--------:|
| 1/2/2008 | 1447.16   | 84.86 | 78.47 | 15.18 | 1.4717  |
| 1/3/2008 | 1447.16   | 85.57 | 78.37 | 15.29 | 1.4745  |
| 1/4/2008 | 1411.63   | 85.13 | 77.31 | 15.17 | 1.4755  |
| 1/7/2008 | 1416.18   | 84.77 | 75.50 | 15.05 | 1.4683  |
| 1/8/2008 | 1390.19   | 86.78 | 76.06 | 15.59 | 1.5571  |

---

## 🛠️ Tech Stack  

- **Python 3.x**
- **Pandas / NumPy** – Data handling  
- **Matplotlib / Seaborn** – Visualization  
- **Scikit-learn** – Machine Learning (Linear Regression, Random Forest, etc.)  
- **XGBoost / LSTM (optional)** – Advanced models for prediction  
- **Jupyter Notebook** – Development & analysis  

---

## 🚀 Workflow  

```mermaid
flowchart TD
    A[📂 Load Financial Dataset] --> B[🧹 Data Preprocessing]
    B --> C[📊 Exploratory Data Analysis]
    C --> D[⚙️ Feature Engineering]
    D --> E[🤖 Model Training - Regression Models]
    E --> F[📈 Model Evaluation - RMSE, R²]
    F --> G[💾 Save Best Model]
    G --> H[🌐 Deploy Model for Prediction]
    H --> I[💰 Predict Future Gold Prices]
