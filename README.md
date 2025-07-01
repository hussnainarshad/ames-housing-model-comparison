# 🏠 Ames Housing Model Comparison

This project applies and compares traditional ML and deep learning models on the [Ames Housing dataset](https://www.kaggle.com/datasets/prevek18/ames-housing-dataset). It demonstrates end-to-end preprocessing, feature engineering, and performance evaluation of:

- 🌲 Random Forest Regressor
- 💡 Support Vector Machine (SVR)
- 🧠 1D Convolutional Neural Network (CNN-1D)
- 🔁 Recurrent Neural Network (RNN / LSTM)

---

## 📊 Model Performance Summary

| Model           | RMSE       | R² Score |
|----------------|------------|----------|
| Random Forest  | 25,108     | 0.9214   |
| CNN-1D         | 67,488     | 0.4319   |
| SVM            | 84,714     | 0.1049   |
| RNN (LSTM)     | 208,871    | -4.4415  |

🟢 **Random Forest** performed best.  
🔴 RNN underperformed due to poor suitability for tabular data in this context.

---

## 📦 Features

- Cleaned and engineered features from raw CSV
- Used `ColumnTransformer` with `StandardScaler` and `OneHotEncoder`
- Applied traditional ML and deep learning models
- Evaluated using RMSE and R²

---

## 🛠️ Requirements

```bash
pip install numpy pandas scikit-learn matplotlib seaborn tensorflow
