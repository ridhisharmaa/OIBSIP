# Car Price Prediction

This project builds a regression model that predicts the selling price of a used car based on things like brand, age, mileage, fuel type, and transmission.

## Dataset

`car_data.csv` has the following columns:
- name
- year
- selling_price
- km_driven
- fuel
- seller_type
- transmission
- owner

Note: The original brief pointed to the "Vehicle dataset from cardekho" on Kaggle. Since I couldn't access Kaggle directly, I generated a dataset with the same column structure and realistic pricing patterns (older cars and higher mileage lower the price, diesel/automatic push it up a bit, etc.), including some messy bits like duplicate rows and inconsistent casing in the fuel column, so the notebook has real cleaning work to do. If you want to use the actual Kaggle dataset instead, just download it and save it with the same filename — the notebook will work the same way.

## What's in the notebook

- Loading the data
- Data cleaning: nulls, duplicates, inconsistent categorical text
- Feature engineering: car age from year, brand extracted from name
- EDA: price distribution, price vs fuel type, price vs car age
- One-hot encoding of categorical columns
- Correlation heatmap
- Train/test split
- Two models trained: Linear Regression and Random Forest Regressor
- MAE, RMSE, and R² for both models
- Feature importance chart for the best model

## How to run

1. Install the required packages:
   ```
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
2. Keep `car_data.csv` in the same folder as the notebook.
3. Open `car_price_prediction.ipynb` in Jupyter Notebook or JupyterLab.
4. Run all cells from top to bottom.

## Result

Random Forest beat Linear Regression on this data (higher R², lower error). Car age and km driven were the two biggest factors in predicting the selling price.
