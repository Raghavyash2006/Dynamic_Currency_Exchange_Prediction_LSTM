# Dynamic Currency Exchange Prediction using Multi-Layer LSTM Networks

## 📌 Project Overview

This project predicts foreign currency exchange rates using a Multi-Layer Long Short-Term Memory (LSTM) neural network. Historical exchange rate data is used to train separate models for multiple currencies. The project demonstrates how deep learning can be applied to time-series forecasting.

---

## 🎯 Project Objectives

- Predict future currency exchange rates using historical data.
- Implement a Multi-Layer LSTM model for time-series forecasting.
- Train separate models for multiple currencies.
- Evaluate model performance using standard regression metrics.
- Visualize actual and predicted exchange rates.

---

## 🌍 Supported Currency Pairs

The project trains separate models for:

- EUR → USD
- EUR → GBP
- EUR → INR

---

## 📂 Dataset

**Dataset Name:** `daily_forex_rates.csv`

### Dataset Columns

| Column | Description |
|--------|-------------|
| currency | Target currency code |
| base_currency | Base currency (EUR) |
| currency_name | Full name of the currency |
| exchange_rate | Historical exchange rate |
| date | Date of exchange rate |

The dataset contains historical exchange rates of multiple currencies with EUR as the base currency.

---

## 🛠 Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Google Colab

---

## 🧠 Model Architecture

The project uses a Multi-Layer LSTM Network with the following architecture:

Input Layer

↓

LSTM (100 Units)

↓

Dropout (0.2)

↓

LSTM (50 Units)

↓

Dropout (0.2)

↓

Dense (25 Units)

↓

Dense (1 Unit)

---

## 🔄 Project Workflow

1. Load Dataset
2. Data Exploration
3. Data Preprocessing
4. Feature Selection
5. Data Normalization using MinMaxScaler
6. Sequence Generation (60 Previous Days)
7. Train-Test Split (80:20)
8. Data Reshaping for LSTM
9. Multi-Layer LSTM Model Training
10. Prediction
11. Performance Evaluation
12. Visualization
13. Save Trained Models

---

## 📊 Evaluation Metrics

The model is evaluated using:

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)

The trained models achieved low prediction errors, indicating good forecasting performance.

---

## 📈 Results

For each currency:

- A separate Multi-Layer LSTM model is trained.
- Actual vs Predicted exchange rate graphs are generated.
- Evaluation metrics are calculated.
- The trained model is saved for future use.

---

## 📁 Project Structure

```
Dynamic-Currency-Exchange-Prediction/
│
├── Dynamic_Currency_Exchange_Prediction_LSTM.ipynb
├── daily_forex_rates.csv
├── README.md
├── requirements.txt
│
└── models/
    ├── USD_lstm_model.keras
    ├── GBP_lstm_model.keras
    └── INR_lstm_model.keras
```

---

## ▶️ How to Run

1. Clone the repository.
2. Install the required libraries:

```bash
pip install -r requirements.txt
```

3. Open the notebook in Google Colab or Jupyter Notebook.

4. Upload the dataset (`daily_forex_rates.csv`).

5. Run all notebook cells.

The notebook will:

- Train separate models for USD, GBP, and INR.
- Display Actual vs Predicted graphs.
- Print evaluation metrics.
- Save the trained models.

---

## 🚀 Future Improvements

- Support additional currency pairs.
- Compare LSTM with GRU and Bi-LSTM models.
- Perform hyperparameter tuning.
- Integrate real-time forex data APIs.
- Develop a web dashboard for live predictions.

---

## 👨‍💻 Author

**Raghav Agarwal**

B.Tech (Artificial Intelligence & Machine Learning)

GLA University, Mathura

---

## 📄 License

This project is developed for educational and academic purposes.