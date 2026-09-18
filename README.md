# CodeAlpha_SalesPrediction

**Data Science Internship — CodeAlpha | Task 4: Sales Prediction using Python**

## 📌 Project Overview
This project predicts product sales based on advertising spend across three channels — TV, Radio, and Newspaper — and quantifies which channel has the strongest impact on sales.

## 📂 Repository Structure
```
CodeAlpha_SalesPrediction/
├── data/
│   └── Advertising.csv
├── plots/
│   ├── correlation_heatmap.png
│   ├── scatter_features.png
│   ├── feature_impact.png
│   └── actual_vs_predicted.png
├── Sales_Prediction.ipynb    # Main notebook
└── README.md
```

## 🛠 Tools & Libraries
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn (LinearRegression, RandomForestRegressor, train_test_split, evaluation metrics)

## 🔍 Workflow
1. **Data Loading & Cleaning** — dropped the unnamed index column, checked for nulls (none found)
2. **EDA** — correlation heatmap and per-channel scatter plots against Sales
3. **Train/Test Split** — 80/20 split
4. **Modeling** — trained and compared Linear Regression and Random Forest Regressor
5. **Evaluation** — R², MAE, RMSE
6. **Feature Impact Analysis** — interpreted linear regression coefficients to rank channel effectiveness

## 📊 Key Results
- **Random Forest Regressor** achieved the best performance: **R² ≈ 0.98**, outperforming Linear Regression (R² ≈ 0.90)
- **TV** has the strongest raw correlation with Sales (≈ 0.78); **Radio** has the highest marginal impact per dollar spent
- **Newspaper** advertising shows almost no measurable effect on sales — a candidate for budget reallocation
- Business takeaway: prioritizing TV and Radio spend over Newspaper is likely to yield better sales returns

## ▶️ How to Run
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook Sales_Prediction.ipynb
```

## 🎓 Internship
Completed as part of the **CodeAlpha Data Science Internship**.
