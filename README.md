# 🚗 AutoPrice — Automotive Pricing Intelligence & Sales Optimization

## 🎯 Project Overview

**AutoPrice** is a data-driven **used-car pricing intelligence system** that predicts optimal selling prices and helps dealers identify **overpriced and underpriced vehicles** using machine learning and business analytics.

It transforms historical vehicle data into actionable **pricing insights and business KPIs**.

## 📸 Visual Preview

![AutoPrice Dashboard](images/dashboard-preview.png)

## 💡 The Problem & Core Value

- 💰 Used-car pricing often relies on inconsistent manual estimates.
- 📉 Overpricing can increase inventory holding time, while underpricing can reduce profit.
- 🤖 AutoPrice uses **historical sales data + machine learning** to create standardized pricing estimates.
- 📊 Compares predicted prices with dealer prices to support faster pricing decisions.

## ✨ Key Features & User Flow

- 🧹 **Automated Data Pipeline** — Handles cleaning, encoding, and scaling using Scikit-learn.
- 📈 **Price Prediction** — Uses Linear Regression to estimate vehicle resale prices.
- 🏷️ **Pricing Intelligence** — Flags vehicles as **Overpriced** or **Underpriced**.
- 📊 **Business KPIs** — Tracks price accuracy, inventory turnover, and profit margin.

**User Flow:**

`Vehicle Data → Preprocessing → Feature Engineering → ML Prediction → Price Comparison → Business Insights`

## 🛠️ Tech Stack & Architecture Decisions

| Layer | Technology | Purpose |
|---|---|---|
| Language | **Python** | Core development |
| Data Processing | **Pandas, NumPy** | Data cleaning & transformation |
| ML Pipeline | **Scikit-learn** | Preprocessing & modeling |
| Prediction Model | **Linear Regression** | Used-car price prediction |
| Visualization | **Matplotlib, Seaborn** | EDA & insights |
| Business Intelligence | **Power BI** | Management dashboards |

## 📈 Challenges & Technical Takeaways

**The Obstacle**
- Vehicle pricing depends on multiple factors such as **age, fuel type, transmission, and historical pricing**.
- Raw data required consistent preprocessing before model training.

**The Resolution**
- Built a reproducible **Scikit-learn preprocessing pipeline**.
- Engineered **Car Age** from manufacturing year.
- Used Linear Regression as a baseline pricing model.
- Achieved an **R² score of ~0.85**.
- Added a pricing decision layer to identify **Overpriced vs Underpriced** vehicles.

## ⚙️ Quick Start

```bash
git clone <your-repository-url>
cd AutoPrice
pip install -r requirements.txt
python train_model.py
```
