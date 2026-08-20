# House Price Prediction using Linear Regression

A Machine Learning project that uses **Linear Regression** to predict residential property sale prices based on various property characteristics.

## Project Overview

The goal of this project is to analyze historical real estate data and build a regression model capable of predicting house prices based on features such as:

* Lot area
* Building type
* Overall condition
* Year built
* Year remodeled
* Exterior type
* Basement area
* Zoning classification
* Lot configuration

## Data Visualization

Exploratory Data Analysis was performed using **Seaborn** and **Matplotlib**.

The project includes visualizations such as:

* **Year Built vs Sale Price** — Scatter Plot
* **Overall Condition vs Sale Price** — Box Plot
* **Building Type vs Sale Price** — Box Plot

These visualizations help identify relationships, trends, and outliers within the dataset.

## Data Preprocessing

Before training the model:

* Rows with missing `SalePrice` values were removed.
* Categorical features such as `MSZoning`, `LotConfig`, `BldgType`, and `Exterior1st` were encoded into numerical values.
* Remaining missing feature values were replaced with `-1`.
* The dataset was divided into **80% training data** and **20% testing data**.

## Model

The project uses:

**Linear Regression**

```python
model = LinearRegression()
model.fit(X_train, y_train)
```

The model is trained using the property features and then used to predict house sale prices from the test dataset.

## Model Performance

The model was evaluated using the **R² Score**.

```text
R² Score: 59.96%
```

This means that the model explains approximately **60% of the variation in house sale prices** using the selected features.

## Technologies Used

* Python
* Pandas
* NumPy
* Seaborn
* Matplotlib
* Scikit-learn
* Jupyter Notebook


## Project Structure

```text
House-Price-Prediction/
│
├── Data/
│   └── real_estate_prices.csv
│
├── real_estate_pp.ipynb
└── README.md
```
