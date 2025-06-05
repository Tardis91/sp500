# Financial Econometrics Analysis of the S&P 500

This analysis applies core financial econometrics techniques to simulated weekly S&P 500 returns (2015–2024).

---

## 📉 Step 1: Log Returns

We analyze log returns to ensure stationarity and apply time series modeling.

---

## 🧪 Step 2: Stationarity Test (ADF)

The Augmented Dickey–Fuller test checks for a unit root.

- **p-value**: `1.16e-23`
- ✅ The series is **stationary** (reject null hypothesis of unit root)

---

## 🔄 Step 3: Autocorrelation Diagnostics

These plots guide ARMA model selection.

### Autocorrelation Function (ACF)

![ACF](images/sp500_acf.png)

---

### Partial Autocorrelation Function (PACF)

![PACF](images/sp500_pacf.png)

---

## 📊 Step 4: ARMA(1,1) Model Results

We estimate an ARMA(1,1) using `ARIMA(1, 0, 1)`:

