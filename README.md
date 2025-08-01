# Car Price Prediction using Machine Learning

This project aims to predict the **selling price** of a used car based on several features such as its current market price, fuel type, seller type, transmission type, and how much it has been driven.

The model helps individuals or businesses in the used car market estimate fair car prices using supervised machine learning.

---


---

## Dataset

- **Source**: open-source used car listings
- **Features**:
  - `Car_Name`
  - `Year`
  - `Selling_Price` *(Target)*
  - `Present_Price`
  - `Kms_Driven`
  - `Fuel_Type`
  - `Seller_Type`
  - `Transmission`
  - `Owner`

- **Target Variable**: `Selling_Price` (continuous value)

---

## Model Workflow

1. **Data Preprocessing**
   - Dropping irrelevant columns
   - Handling categorical variables using `pd.get_dummies`
   - Feature engineering (e.g., calculating car age)

2. **Train-Test Split**
   - 80% training, 20% testing

3. **Model Used**
   - `RandomForestRegressor`, `GradientBoostingRegressor` from `sklearn` and `XGBRegressor` from `xgboost`

4. **Model Evaluation**
   - Metrics: MAE, MSE, RMSE, R² score

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Reyad02/car-price-prediction.git
   cd car-price-prediction 
   ```
   
2. Install dependencies:
   ```bash
    pip install -r requirements.txt
   ```

3. Run the Jupyter notebook:
   ```bash
    jupyter notebook main.ipynb
   ```

