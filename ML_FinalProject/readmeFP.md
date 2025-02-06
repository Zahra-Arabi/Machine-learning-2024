📌 Final Project README (ML_FinalProject/README.md)

# Final Machine Learning Project - Stock Price Prediction

## 📌 Project Overview
This project explores **stock price prediction** using various **machine learning** and **deep learning models**. The dataset includes **historical stock prices, market indicators, macroeconomic factors, and sentiment analysis data**. Several models were tested, including **LSTM, GRU, CNN-LSTM, Transformer, MLP, and ANFIS**.

## 📂 Repository Structure

ML_FinalProject/ │── code/ │ ├── Stock_Forecasting_Project.ipynb # Jupyter Notebook with model implementation │── data/ │ ├── comprehensive_stock_data.xlsx # Processed dataset for model training │── report/ │ ├── ZahraArabi_40007173_Project.pdf # Official project report │── README.md # Project description
---

## 📊 **Dataset and Features**
### **Data Sources**
- **Yahoo Finance API** → **Stock Prices (Open, Close, High, Low, Volume)**
- **Finnhub API** → **Sentiment Analysis from Financial News**
- **FRED API** → **Macroeconomic Indicators (GDP, Inflation, Unemployment)**
- **Options Market Data** → **Put/Call Ratios, Trading Volumes**

### **Key Features**
- **Stock Market Data**: S&P 500, NASDAQ, Dow Jones.
- **Economic Indicators**: GDP, CPI, Unemployment Rate, Interest Rates.
- **Sentiment Analysis**: News sentiment scores.
- **Options Data**: Call/Put volumes, Put/Call ratio.
- **Technical Indicators**: Moving Averages, Volatility, Price Changes.

### **Data Preprocessing**
✔ Removed **missing values** and **outliers**.  
✔ Applied **MinMax Scaling** and **Standardization**.  
✔ Transformed **time-series data into sequences** for LSTM-based models.  
✔ Engineered **new features** such as **moving averages, volatility, and market sentiment**.  

---

## 🛠 **Models Used**
### **1️⃣ Long Short-Term Memory (LSTM)**
- Captures long-term dependencies in sequential data.
- Struggles with **overfitting** in limited data scenarios.

### **2️⃣ Gated Recurrent Unit (GRU)**
- Similar to LSTM but computationally efficient.
- Best performance in terms of **accuracy and generalization**.

### **3️⃣ CNN-LSTM Hybrid Model**
- Extracts features using CNN before LSTM processing.
- Had issues with **overfitting** and complex computations.

### **4️⃣ Transformer Model (Attention Mechanism)**
- Parallel processing improves efficiency.
- Struggled with **short-sequence financial data**.

### **5️⃣ Multi-Layer Perceptron (MLP)**
- Basic model but failed to capture time dependencies.

### **6️⃣ Adaptive Neuro-Fuzzy Inference System (ANFIS)**
- Combined **fuzzy logic with neural networks**.
- Performed **better than MLP** but still had instability.

---

## 📊 **Results & Model Comparison**
| Model | RMSE (Test) | MAE (Test) | R² Score |
|------|------|------|------|
| **GRU** | **25.20** | **14.34** | **0.65** |
| **LSTM** | 28.30 | 16.50 | 0.58 |
| **CNN-LSTM** | 33.40 | 32.10 | -0.03 |
| **Transformer** | 30.50 | 19.80 | 0.45 |
| **MLP** | 36.00 | 34.00 | -0.15 |
| **ANFIS** | 31.80 | 26.70 | 0.30 |

### **🏆 Best Model: GRU**
- **Lowest RMSE & MAE**.
- **Best generalization** to unseen test data.
- **Handled stock price fluctuations effectively**.

### **📉 Worst Model: MLP**
- **Poor accuracy** with **negative R²**.
- **Unable to capture time dependencies**.

---

## 🚀 **How to Run the Project**
1. **Clone the repository**:
   ```bash
   git clone https://github.com/Zahra-Arabi/Machine-learning-2024.git
   cd Machine-learning-2024/ML_FinalProject
Open the Jupyter Notebook (Stock_Forecasting_Project.ipynb) in:

Google Colab (Recommended)
Jupyter Notebook
Run all cells and follow the explanations in the notebook.

📌 Google Colab Link:
🔗 **[COLAB FINAL PROJECT](https://colab.research.google.com/drive/10_l21YcWot8c63YOCukeXIyUMoWW_IrU?usp=sharing)**

📄 Related Files
📜 Final Report
📊 Dataset



👩‍💻 Author
Name: Zahra Arabi
University: K. N. Toosi University of Technology
Instructor: Dr. Mahdi Aliyari
🚀 Happy Coding! 🎯
