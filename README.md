
# HRC Price Forecasting Dashboard

## 📘 Project Overview

This project is developed in collaboration with **TATA Steel** as part of the **BT4103 Business Analytics Capstone Project** at the **National University of Singapore**.

Our goal is to build an interactive forecasting dashboard to project **Hot Rolled Coil (HRC)** export prices from **China** and **Japan/Korea** for the year **2025**. The dashboard supports TATA Steel’s strategic pricing decisions by integrating economic drivers and forecasting models.

The dashboard also features an **Import Parity Landed Price Calculator** to estimate the competitiveness of imported steel in India compared to domestic pricing.

---

## 🔍 Key Features

- **Forecasting Models**
  - Vector Autoregression (VAR)
  - Multiple Linear Regression
  - Long Short-Term Memory (LSTM)

- **Country Support**
  - China
  - Japan

- **Forecast Drivers**
  - Iron ore, coking coal, and scrap prices
  - Export volumes
  - Fixed Asset Investment (FAI)

- **Landed Price Calculator**
  - Computes Indian import parity prices based on user inputs (FOB, CIF, duties)

- **Interactive Dashboard**
  - Built with Streamlit
  - Forecast charts with export options (CSV, PNG)
  - Selectable model type and time range

---

## 🛠️ How to Run the Dashboard

### 1. Clone the Repository

```bash
git clone https://github.com/Tinatianye/BT4103-Business-Analytics-Capstone-Project.git
cd BT4103-Business-Analytics-Capstone-Project
```

### 2. Install Required Packages

It is recommended to use a virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # For Linux/Mac
venv\Scripts\activate     # For Windows

pip install -r requirements.txt
```

If you don’t have a `requirements.txt` yet, you can generate one:

```bash
pip freeze > requirements.txt
```

### 3. Run the App

```bash
streamlit run app.py
```

### 4. Open in Browser

Once the app starts, Streamlit will automatically open a browser window (usually at http://localhost:8501). If not, open it manually.

---

## 📁 Project Structure

```
├── app.py                             # Main Streamlit dashboard
├── china_japan.py                    # Forecast generation logic
├── 02_var.ipynb                      # VAR model development
├── 04_multiple_regression.ipynb     # Regression model development
├── 05_hrc_price_Japan_prediction.ipynb # Japan-specific LSTM model
├── 06_china_japan_forecast.ipynb    # Unified forecast plotting
├── data/                             # Optional: data files directory
├── requirements.txt                  # Python dependencies
└── README.md                         # Project documentation
```

---

## 📊 Data Sources

- Raw material prices (iron ore, coking coal, scrap)
- Export volumes and FAI statistics
- Internal forecast outputs from project notebooks

**Note**: All data used is for academic research purposes only.

---

## 🧠 Methodology Summary

- Macroeconomic factor integration
- Upside and downside scenario modeling
- Forecast uncertainty visualization
- Comparative model analysis (VAR, Regression, LSTM)

---

## 🤝 Acknowledgements

This project was completed as part of the NUS BT4103 Capstone module in partnership with **TATA Steel**. Special thanks to our academic advisors and industry mentors for their valuable support and insights.

---

