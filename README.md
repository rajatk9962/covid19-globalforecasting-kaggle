# **COVID-19 Case Prediction**

## Introduction

This project was developed as part of a **Kaggle competition** where the goal was to predict the number of **confirmed COVID-19 cases** and **fatalities** over time. The dataset provided included historical records of cases and deaths across various countries.

A **Polynomial Regression model** was used to forecast future cases and fatalities based on historical trends.

## 📊 Dataset

The dataset for this competition was provided by **Kaggle** under the **COVID-19 Global Forecasting** competition:

- **Train Data:** `train.csv`
- **Test Data:** `test.csv`
- **Submission Format:** `submission.csv`

Each record contains:
- `Date`: The date of the record.
- `Country/Region`: The location where cases are reported.
- `ConfirmedCases`: The cumulative number of confirmed cases.
- `Fatalities`: The cumulative number of fatalities.

The data was preprocessed to separate **cases** and **fatalities** into structured CSV files.

---

## Model Used

- **Polynomial Regression (degree = 4)**
  - The dataset was processed and split into separate CSV files for **cases** and **fatalities**.
  - A **polynomial regression model** was trained on each country's cases and fatalities data.
  - Predictions were made for future days and stored in a submission file.

---

## Installation

Ensure you have **Python 3** installed. The following dependencies are required:

```bash
pip install numpy pandas scikit-learn matplotlib
```
## Results
 - The Polynomial Regression model was able to predict the number of COVID-19 cases and fatalities across different countries.
 - The final predictions were saved in submission.csv for submission on Kaggle.
 - Further improvements can be made using time-series models like LSTMs, ARIMA, or Prophet.
