# 🏠 House Price Prediction using Linear Regression

A Machine Learning project that predicts house prices using linear regression, based on features like square footage, lot size, and garage size. The model is built using Python and scikit-learn.

---

## 🎯 Objective

The goal of this project is to build an interpretable regression model to predict the **log-transformed house price** using key numerical features. We aim to achieve high accuracy while keeping the model simple and explainable.

---

## 📂 Dataset

The dataset contains **1000 rows** with the following columns:

- `Square_Footage` – Total floor area
- `Num_Bedrooms` – Number of bedrooms
- `Num_Bathrooms` – Number of bathrooms
- `Lot_Size` – Size of the plot in acres
- `Garage_Size` – Garage capacity (number of cars)
- `Neighborhood_Quality` – A numeric score (1 to 10)
- `House_Price` – Price of the house in USD

---

## 🧼 Data Preprocessing

- ✅ No missing values found
- ✂️ Dropped low-correlation features:
  - `Num_Bedrooms`
  - `Num_Bathrooms`
  - `Neighborhood_Quality`
- 🔄 Applied `log()` transformation on `House_Price` → `Log_House_Price`
- ⚙️ Final features used: `Square_Footage`, `Lot_Size`, `Garage_Size`

---

## 📊 Exploratory Data Analysis (EDA)

- ✅ Strong positive correlation between `Square_Footage` and house price
- ❌ Weak correlation from bedroom/bathroom count and neighborhood score
- 📈 Used Seaborn heatmaps for visualizing feature correlation

---

## 🔁 Train/Test Split

- `train_test_split(test_size=0.2, random_state=42)`
- 80% for training, 20% for testing
- Target variable: `Log_House_Price`

---

## 🤖 Model Used

- ✅ Algorithm: **Linear Regression**
- 🔧 Library: `scikit-learn`
- 🧠 Model learned from `Square_Footage`, `Lot_Size`, and `Garage_Size`

---

## 📈 Model Evaluation

### ✅ Test Set Performance:

- 📉 **MAE**: 0.0966  
- 📉 **RMSE**: 0.1246  
- 📈 **R² Score**: 0.935

### ✅ Training Set Performance:

- 📉 **MAE**: 0.1016  
- 📉 **RMSE**: 0.1326  
- 📈 **R² Score**: 0.927

✅ The model is **well-fitted** and **not overfitted** — performance is consistent on both training and test sets.

---

## 📉 Visualization

![Actual vs Predicted](https://github.com/user-attachments/assets/c590197d-8cbf-4a7e-8ab9-b3a2e86fae31)



---

## 💡 Conclusion

- Linear Regression performed excellently with minimal features
- Log transformation improved accuracy and interpretability
- A simple model can perform impressively with the right preprocessing

---

## 🚀 Future Work

- Add Ridge or Lasso Regression for regularization
- Try Polynomial Regression for non-linearity
- Build a web app using Streamlit for interactive predictions
- Include categorical features like location, property type, etc.

---

## 🧠 Skills Used

- Data Cleaning & Feature Selection
- Exploratory Data Analysis
- Linear Regression
- Model Evaluation
- Data Visualization

---

## 💬 Author

**Thrisha**  
🎓 B.Tech Artificial Intelligence & Data Science  
👑 ML | Pythonista | Creative Technophile  

- 💼 [LinkedIn](https://www.linkedin.com/in/thrisha-s-299970266)

---

> "Code with logic. Train with passion. Predict with purpose." — Thrisha
