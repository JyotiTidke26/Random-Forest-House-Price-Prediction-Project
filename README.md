# 🏡 Random Forest Regressor for House Price Prediction

## 📌 Project Description

In this project, we aim to predict house prices using the **[House Sales in King County, USA](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction)** dataset. The workflow begins with data collection and is followed by detailed data assessment, cleaning, and exploratory data analysis (EDA). These steps help in understanding the structure of the dataset and identifying patterns that are crucial for predictive modeling.

The core of this project lies in the implementation of the **Random Forest Regressor**, an ensemble learning algorithm known for its robustness, ability to handle mixed data types, and resistance to overfitting. It is particularly effective in modeling complex, non-linear relationships in real-world data.

## 📌 Overview

We use a **Random Forest Regressor** to model and predict house prices. The pipeline includes:
- ✅ Data preprocessing  
- ✅ Feature selection  
- ✅ Model training  
- ✅ Hyperparameter tuning using **GridSearchCV**  
- ✅ Evaluation using standard regression metrics  
- ✅ Visualization of feature importance and prediction results  

---

## 📂 Dataset

The dataset used for this project is publicly available on [Kaggle](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction). It includes records of house sales with the following features:

- `price` — 💰 House price *(target variable)*
- `bedrooms`, `bathrooms` — 🛏️ Number of bedrooms & 🛁 bathrooms
- `sqft_living`, `sqft_lot` — 📐 Living area and lot area in square feet
- `floors` — 🏠 Number of floors
- `waterfront`, `view` — 🌊 Whether house is waterfront and view quality
- `condition`, `grade` — 🧱 Overall condition and construction grade
- `sqft_above`, `sqft_basement` — 📏 Above-ground and basement square footage
- `lat`, `long` — 📍 Latitude and longitude coordinates
- `sqft_living15`, `sqft_lot15` — 📆 Living and lot area in 2015
- `year`, `month` — 📅 Sale year and month
- `house_age` — ⌛ Age of the house
- `is_renovated` — 🔧 Renovation status (binary)

---

## 🛠️ Why Random Forest?

Random Forest was chosen because it:
- 🌳 Is a powerful ensemble learning method that reduces overfitting common in decision trees
- 🔍 Handles both numerical and categorical data effectively
- 💪 Performs well on large datasets and can model complex relationships
- 🧠 Automatically captures feature importance

---

## 🧪 Modeling Approach

1. **Data Preprocessing**:
   - Handled missing values  
   - Converted features into appropriate formats  
   - Engineered new features like `house_age` and `is_renovated`  
2. **Model Selection**:
   - Trained a **Random Forest Regressor**  
   - Tuned hyperparameters (`n_estimators`, `max_depth`, `min_samples_split`, etc.) using **GridSearchCV**  
3. **Evaluation**:
   - Assessed model using standard metrics (MAE, MSE, RMSE, R²)  
   - Visualized predictions and feature importances  

---

## 📈 Model Performance

The final tuned Random Forest Regressor achieved the following evaluation results:

| Metric        | Score               |
|---------------|---------------------|
| ✅ MAE         | 50,576.49            |
| ✅ MSE         | 5,475,873,409.93     |
| ✅ RMSE        | 73,999.14            |
| ✅ R-squared   | 0.856                |

🔍 *The R² score of 0.856 indicates that the model explains approximately 85.6% of the variance in house prices, making it a strong predictor for this regression task.*

---

## 📄 License

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.
