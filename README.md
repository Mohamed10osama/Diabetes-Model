# Diabetes Disease Progression Prediction

A machine learning project that predicts diabetes disease progression using the Scikit-learn Diabetes dataset. Two models are trained and compared: XGBoost and Random Forest.

---

## Dataset

- **Source:** Scikit-learn built-in `load_diabetes()`
- **Samples:** 442 patients
- **Features:** 10 (age, sex, bmi, bp, s1–s6)
- **Target:** Disease progression score one year after baseline

---

## Project Steps

1. **EDA** — target distribution, feature distributions, correlation heatmap
2. **Modeling** — XGBoost and Random Forest regressors
3. **Evaluation** — MAE, R², RMSE
4. **Feature Importance** — which features matter most
5. **Actual vs Predicted plot** — visual model performance check

---

## Results

| Model | MAE | R² | RMSE |
|---|---|---|---|
| XGBoost | 46.39 | 0.37 | 57.89 |
| Random Forest | 44.05 | 0.44 | 54.33 |

**Random Forest outperforms XGBoost on all metrics.**

Key finding: `bmi` and `s5` are the most important features according to XGBoost feature importance.

---

## How to Run

Install dependencies:

```bash
pip install pandas matplotlib seaborn scikit-learn xgboost
```

Run the script:

```bash
python diabetes_model.py
```

---
