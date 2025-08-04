# ✈️ Flight Fare Analysis, Prediction & Dashboard (Python + Power BI)

This project is a complete flight fare analysis and prediction solution, combining **Exploratory Data Analysis (EDA)**, a **Machine Learning Price Prediction Model**, and a dynamic **Power BI Dashboard**.

---

## 📌 Project Overview

The goal of this project is to:
- Understand pricing trends in flight ticket data,
- Predict future ticket prices using machine learning,
- Visualize trends through a clean and interactive Power BI dashboard.

---

## 🎯 Objectives

- Perform end-to-end EDA on flight fare data.
- Build and evaluate a flight fare **prediction model**.
- Create a business-friendly **Power BI dashboard**.
- Uncover pricing patterns, booking behavior, and airline differences.
- Deliver real-time insights using slicers, KPIs, and conditional formatting.

---

## 🧠 Machine Learning Price Prediction

I built a **supervised regression model** using Python to predict flight prices based on historical features.

### ✳️ ML Workflow:
- **Data Preprocessing**: 
  - One-hot encoding, label encoding, datetime transformation
  - Feature engineering (days left, route, duration, class)
- **Model Selection**: 
  - Compared **Linear Regression, Random Forest, XGBoost**
- **Best Model**: 
  - **Random Forest Regressor** with GridSearchCV for hyperparameter tuning
- **Performance**:
  - RMSE: ~4530.30
  - R² Score: 0.9602 (on test data)



### 🔢 Features Used:
| Feature | Description |
|---------|-------------|
| `airline` | Categorical |
| `source_city` / `destination_city` | Route indicators |
| `departure_time` / `arrival_time` | Binned for time of day |
| `days_left` | Days until flight |
| `class` | Economy or Business |
| `duration` | Total flight time in minutes |

📦 Target: `price`

<img width="1436" height="804" alt="Screenshot 2025-08-04 112833" src="https://github.com/user-attachments/assets/70ee0007-96d6-49e2-b08a-2a8e564314da" />


---

## 📊 Power BI Dashboard Features

✅ **KPI Cards**:
- Total Flights, Avg Fare, Max Fare, Min Fare

✅ **Visuals**:
- Bar charts: Avg Fare by Airline, Class, Route
- Heatmap: Source vs Destination
- Table: High fares (highlighted in red)
- Top 5 Expensive Routes
- Class vs Price distribution
- Route Fare Summary

---

<img width="1433" height="804" alt="Screenshot 2025-08-04 112932" src="https://github.com/user-attachments/assets/677d4e9b-6f9f-403a-b069-06f1de285a2f" />


## 🔍 Key Questions Answered

1. Which airline is the most affordable?
2. How do business class and economy fares compare?
3. Do last-minute bookings cost more?
4. What’s the impact of flight duration on price?
5. Which city pairs are the most expensive?
6. How accurate is our model in predicting fare?
7. Which features influence pricing the most?

---

## 🧰 Tools & Technologies Used

| Tool | Purpose |
|------|---------|
| Python (Pandas, NumPy, Seaborn, Scikit-learn) | EDA + ML Modeling |
| Power BI | Business Dashboard |
| Excel | Data Formatting |
| DAX | Calculated Columns & Measures |
| GitHub | Version Control & Portfolio Hosting |

---

## 💼 Business Insights

- **Fare increases by 32%** when booked 1–2 days before departure.
- **Business class** has high volatility—up to **8x costlier** than economy.
- **XGBoost and Random Forest** perform well in modeling complex relationships between route, duration, and fare.
- Predictive accuracy is strongest for economy tickets booked well in advance.

---



