# 📊 Milestone 2 – Feature Engineering for Azure Usage Forecasting

## Project Overview

This milestone focuses on transforming the cleaned economic dataset into a feature-engineered dataset suitable for time-series forecasting. The objective is to enhance the dataset by creating meaningful temporal and lag-based features that improve predictive performance for Azure usage forecasting.

Feature engineering plays a critical role in preparing structured data for modeling. In this phase, multiple transformations were applied to capture time trends, seasonality, and historical dependencies within the data.

---

## Work Completed

### 1. Dataset Preparation
The cleaned dataset from Milestone 1 was loaded using Pandas. Column names were standardized and the dataset was prepared for transformation.

### 2. Date Feature Creation
A structured monthly Date column was generated using `pd.date_range()` to ensure proper chronological ordering of observations. This enables time-series modeling.

### 3. Time-Based Features
From the Date column, the following features were extracted:
- Year
- Month
- Quarter

These features help capture seasonal patterns and long-term trends in economic indicators.

### 4. Lag Feature Engineering
Lag-1 features were created for numerical variables to capture previous period values.  
Lag features are essential in forecasting problems because they allow the model to learn from historical behavior.

### 5. Sorting & Data Integrity
The dataset was sorted chronologically by Date to maintain time order consistency, which is critical for forecasting.

### 6. Missing Value Handling
Lag feature creation introduces missing values in the first row.  
Backward filling (`bfill()`) was applied to ensure the dataset contains no missing values.

### 7. Final Dataset Export
The final processed dataset was exported as:

`economic_data_feature_engineered.csv`

This dataset is fully prepared for predictive modeling in the next milestone.

---

## Files Included

- `milestone2_feature_engineering.ipynb` – Complete implementation of feature engineering
- `economic_data_feature_engineered.csv` – Final engineered dataset
- `Milestone_2_Report.pdf` – Detailed documentation of the process

---

## Tools & Technologies Used

- Python  
- Pandas  
- NumPy  
- Google Colab  
- GitHub  

---

## Outcome

At the end of Milestone 2:

- The dataset is structured for time-series analysis.
- Temporal features (Year, Month, Quarter) are added.
- Lag-based historical features are created.
- No missing values remain.
- The dataset is ready for model building and forecasting.

Milestone 2 has been successfully completed and the project is ready to move into predictive modeling.
