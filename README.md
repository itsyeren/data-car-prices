# Car Prices — Data Analysis & Price Prediction

A data-science project that analyzes used car sales data and builds predictive models to estimate car selling prices based on key features like age, kilometers driven, fuel type, transmission, and more.

This repository contains an exploratory data analysis and machine learning workflow in a Jupyter Notebook (`Car-Prices.ipynb`), covering data cleaning, visualization, feature engineering, and regression modeling.

---

## 📌 Project Overview

**Goal:**  
Predict the selling price of used cars using supervised learning regression models.

**Motivation:**  
Used car pricing is influenced by many factors. Building a model helps understand how features like age, mileage, and specs affect price — useful for buyers, sellers, and data scientists alike.

---

## 📁 Dataset

The dataset includes listings of used cars with features such as (common from similar projects):  
- `Car_Name` — brand/model  
- `Year` — year of registration  
- `Selling_Price` — target price  
- `Present_Price` — showroom price  
- `Kms_Driven` — distance traveled  
- `Fuel_Type` — Petrol/Diesel/CNG  
- `Seller_Type` — Dealer/Individual  
- `Transmission` — Manual/Automatic  
- `Owner` — number of previous owners:contentReference[oaicite:0]{index=0}

*(If your actual columns differ, update this section to reflect them.)*

---

## 🧠 What’s Inside

The primary notebook `Car-Prices.ipynb` walks through:

1. **Data Loading & Inspection**  
   Check shapes, types, missing values.

2. **Exploratory Data Analysis (EDA)**  
   Visualizing distributions, correlations, trends.

3. **Data Cleaning & Feature Engineering**  
   Handling missing values, encoding categoricals, scaling, derived features.

4. **Modeling & Evaluation**  
   Training and comparing regression models (e.g., Linear Regression, Random Forest, Gradient Boosting).  
   Evaluate with metrics like R², MAE, MSE.

5. **Results & Insights**  
   Which features matter most and model performance comparisons.

---

## 🚀 How to Run Locally

1. **Clone this repo**
    ```bash
    git clone https://github.com/itsyeren/data-car-prices.git
    cd data-car-prices
    ```

2. **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```

3. **Open the notebook**
    ```bash
    jupyter notebook Car-Prices.ipynb
    ```

4. **Follow the workflow in the notebook**  
   Run each cell from top to bottom to reproduce the analysis and model results.

---

## 📦 Requirements

Typical packages used in this type of project:
- Python 3.7+
- pandas
- numpy
- matplotlib / seaborn
- scikit-learn
- jupyter

*(Include an actual `requirements.txt` with versions if you already have one.)*

---

## 🧪 Example Output

After training, your models can be used to estimate a car’s selling price given its features.  
(Mention specific performance numbers here if you have them — e.g. “Random Forest achieved R² of 0.88” — if not yet measured, you can add later.)

---

## 📝 Notes & Future Work

- Add model serialization (`.pkl`) to reuse without retraining.
- Build a simple web app (Streamlit/Flask) for live price prediction.
- Hyperparameter tuning and cross-validation to improve accuracy.

---

## 👤 Author

**itsYeren** — Data enthusiast building ML projects and expanding analytical skills.

---

