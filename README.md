# ReCell: Used Device Price Prediction

<img width="1712" height="682" alt="ReCell image" src="https://github.com/user-attachments/assets/1d2ac582-3839-447a-8780-bad7f6ac4698" />


## Project Overview

The global market for used and refurbished smartphones and tablets has experienced significant growth due to increasing consumer demand for affordable devices and sustainability initiatives. ReCell, a startup operating in this market, aims to develop a data-driven pricing strategy that accurately predicts the resale value of used mobile devices.

This project applies multiple linear regression to analyze the factors that influence the prices of used smartphones and tablets and builds a predictive model that supports dynamic pricing decisions.

---

## Project Highlights

- Developed a multiple linear regression model to predict the resale prices of used smartphones and tablets.
- Achieved an R² score of **0.8425** on the test dataset, indicating strong predictive performance.
- Identified the original retail price, RAM, screen size, camera resolution, and release year as key drivers of resale value.
- Generated actionable business recommendations to support ReCell's dynamic pricing strategy.

---

## Business Objective

The objective of this project is to develop a machine learning model capable of predicting the normalized resale price of used smartphones and tablets while identifying the key factors that significantly influence pricing.

The insights generated will enable ReCell to:

- Develop a consistent pricing strategy
- Improve pricing accuracy
- Reduce manual pricing decisions
- Maximize profitability in the refurbished device market

---

## Dataset

The dataset contains information on used smartphones and tablets, including:

- Brand
- Operating system
- Screen size
- 4G and 5G support
- Main camera resolution
- Selfie camera resolution
- RAM
- Internal memory
- Battery capacity
- Weight
- Release year
- Days used
- Original (new) normalized price
- Normalized used price (target variable)

---

## Project Workflow

1. Data Exploration
   - Dataset overview
   - Missing value analysis
   - Duplicate checks
   - Summary statistics

2. Exploratory Data Analysis (EDA)
   - Univariate analysis
   - Bivariate analysis
   - Correlation analysis
   - Visualizations

3. Data Preprocessing
   - One-hot encoding of categorical variables
   - Train-test split
   - Feature preparation

4. Multiple Linear Regression
   - Initial model development
   - Model refinement
   - Feature significance analysis

5. Assumption Testing
   - Linearity
   - Normality of residuals
   - Homoscedasticity
   - Independence of errors
   - Multicollinearity (Variance Inflation Factor)

6. Model Evaluation
   - Mean Absolute Error (MAE)
   - Root Mean Squared Error (RMSE)
   - R² Score
   - Training vs Testing performance comparison

7. Business Recommendations

---

## Technologies Used

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Statsmodels
- Scikit-learn

---

## Model Performance

Final Model Performance

| Metric | Training | Testing |
|---------|----------|----------|
| MAE | 0.1803 | 0.1841 |
| RMSE | 0.2298 | 0.2383 |
| R² | 0.8449 | 0.8425 |

The similarity between the training and testing metrics indicates that the model generalizes well to unseen data and does not exhibit significant overfitting.

---

## Key Findings

- The model explains approximately **84%** of the variation in used device prices.
- The normalized new price is the strongest predictor of resale value.
- Device specifications such as RAM, screen size, camera resolution, and release year significantly influence resale prices.
- Devices supporting 4G connectivity generally command higher resale values.
- Technical specifications have a greater impact on pricing than brand alone.
- The model demonstrates strong predictive performance on unseen data, making it suitable for supporting pricing decisions.

---

## Business Recommendations

- Use the original retail price as the primary input when estimating resale values.
- Incorporate technical specifications, including RAM, screen size, camera quality, and release year, into pricing decisions.
- Consider network capabilities such as 4G support when valuing used devices.
- Prioritize objective device specifications over brand reputation when determining resale prices.
- Integrate the predictive model into ReCell's pricing workflow to improve pricing consistency and reduce manual decision-making.
- Periodically retrain the model using recent market data to maintain prediction accuracy as technology and consumer preferences evolve.

---

## Repository Structure

```
├── data/
│   └── used_device_data.csv
├── notebooks/
│   └── ReCell_Used_Device_Price_Prediction.ipynb
├── images/
│   └── visualizations
├── README.md
└── requirements.txt
```

---



## Future Improvements

- Compare multiple regression with tree-based machine learning models such as Random Forest, XGBoost, and Gradient Boosting.
- Perform hyperparameter tuning to improve predictive performance.
- Develop an interactive pricing application using Streamlit.
- Deploy the model as a web application for real-time resale price prediction.

---

## Author


- LinkedIn: https://www.linkedin.com/in/irene-kibengo-44964356/
