# 📉 NIFTY 50 Prediction Using Global Macro Indicators

A machine learning project to predict whether the NIFTY 50 index will **rise or fall 1 month into the future**, using a wide range of **global macroeconomic indicators** like crude oil prices, USD/INR, gold, US stock indices, volatility indexes, and more.

---

## 🔍 Goal

- Build a predictive model using **past price trends** and **global indicators**.
- Predict the **1-month future movement** of the NIFTY 50 index:  
  `Rise` (1) or `Fall` (0)

---

## 📊 Data Used

- **NIFTY 50 index historical prices**
- **Macro indicators from Yahoo Finance**, including:
  - Crude oil (`BZ=F`)
  - Gold (`GC=F`)
  - USD/INR (`INR=X`)
  - US indices (`^GSPC`, `^DJI`, `^IXIC`)
  - Volatility Indexes (`^VIX`, `^INDIAVIX`)
  - Bond yields, copper, silver, wheat, etc.

---

## ⚙️ Technologies Used

- **Python 3.9+**
- **Pandas, NumPy**
- **Scikit-learn**
- **XGBoost**
- **SMOTE (for handling class imbalance)**
- **Logistic Regression**
- **Random Forest (exploratory)**
- **Matplotlib, Seaborn (for visualization)**
- **Jupyter Notebook (via Anaconda)**

---

## 🧠 ML Models Tried

We tried a **variety of models** to improve prediction performance:

| Model                 | Tried | Notes                                  |
|----------------------|-------|----------------------------------------|
| Logistic Regression  | ✅    | Baseline, easy to interpret            |
| Random Forest        | ✅    | Non-linear, better than baseline       |
| XGBoost              | ✅    | High-performance, best for tabular data |
| SMOTE + Logistic     | ✅    | Helped balance class labels            |

---

## 📉 Results

- Our **model was able to recall "Fall" cases quite well**, but...
- It **struggled to predict "Rise" cases** accurately.
- Most models **over-predicted Fall**, leading to poor overall precision and imbalance.

---

## 🚧 Challenges Faced

- **Class Imbalance**: Far fewer "Fall" cases than "Rise".
- **Feature Limitations**: Macro indicators are complex and noisy.
- **False Alarms**: High number of false positives for "Fall".
- **Time-series Complexity**: Global factors affect markets unpredictably.

---

## 💡 What We Learned

- Even when models don’t perform well, we learn a lot by:
  - Cleaning, merging, and enriching real-world financial data.
  - Applying advanced ML techniques like **SMOTE**.
  - Evaluating using **classification reports** and **confusion matrices**.
  - Understanding the importance of **feature engineering** in finance.
- Machine learning for stock markets is **hard**, but we gained **a ton of practical insight**.

---

## 🙌 Final Thoughts

This project may not have achieved high accuracy, but:
- I tried **everything we could** — multiple models, balancing methods, and clean data.
- It was a **rich learning experience** in applying ML to real financial data.

---


