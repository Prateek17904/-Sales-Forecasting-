# 🚀 Sales Forecasting Pipeline with Machine Learning

## Quick Start

**An end-to-end notebook for accurate sales forecasting!**

This project provides a complete system to analyze historical data, train a high-performance machine learning model, and predict future sales with over 83% accuracy.

---

## 🎯 What It Does

-   **Analyzes** historical sales data to uncover trends and seasonality.
-   **Predicts** future sales amount ($) for the next 6 months.
-   **Provides** forecasts at both the plant and customer levels.
-   **Generates** a business dashboard with actionable insights.

---

## 🚀 How to Run

### Prerequisites

-   Python 3.9+
-   Jupyter Notebook / JupyterLab

### Installation & Setup

1.  **Place Data:** Ensure `Sales forecasting train data.csv` and `Sales forecasting test data.csv` are in a `data/` folder located one level above your notebook's directory.
2.  **Install Libraries:**
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn xgboost jupyter
    ```
3.  **Run the Notebook:**
    -   Open `notebooks/Sales_Forecasting_Complete.ipynb`.
    -   Click **"Run All"** from the `Cell` menu.
    -   Execution takes approximately 2-5 minutes.
    -   View the final charts, analysis, and output files.

---

## 📊 Expected Results

-   **>83% prediction accuracy** (exceeds 80% requirement).
-   **Plant performance analysis** identifying key revenue drivers.
-   **Top customer forecasts** with concentration risk analysis.
-   **Monthly sales forecasts** highlighting seasonal peaks.
-   **Actionable business recommendations** for strategic planning.

---

## 📈 Key Outputs

After running the notebook, you'll get:

-   `final_predictions.csv` - The main forecast data.
-   `plant_level_forecast.csv` - Aggregated insights by plant.
-   `customer_level_forecast.csv` - Analysis for top customers.
-   A final dashboard visualization within the notebook.

---

## 💡 Business Value

-   **Optimize inventory** and production based on demand forecasts.
-   **Strengthen relationships** with high-value customers.
-   **Allocate resources** effectively across different plants.
-   **Anticipate market trends** and seasonal demand shifts.
-   **Enable data-driven** strategic and financial decisions.

---

## 🔧 Technical Details

-   **Model**: **Random Forest Regressor** (best performer with 83.5% accuracy).
-   **Features**: 25+ engineered features including seasonality (sin/cos), time lags, rolling averages, and statistical aggregations.
-   **Validation**: Robust time-series split (80% train, 20% validation) to prevent data leakage and simulate real-world performance.
-   **Output**: Clean, aggregated forecasts ready for business consumption.

---

## 🛠️ Technology Stack

**Core Libraries:**

-   `pandas` - Data manipulation and analysis.
-   `numpy` - Numerical operations.
-   `scikit-learn` - Machine learning models and utilities.
-   `xgboost` - Used for model comparison.
-   `matplotlib` & `seaborn` - Data visualization.
-   `jupyter` - Interactive development environment.

---

## 📈 Key Insights from EDA

### Data Quality

-   ✅ The dataset is clean with no significant missing values.
-   📊 Contains over two years of historical data, sufficient for trend analysis.
-   🏭 **Plant_2** is the dominant contributor to total sales.

### Temporal Patterns

-   📅 **Strong seasonality** is observed, with sales peaking in the spring months.
-   📈 A clear **upward trend** in overall sales year-over-year.

### Business Insights

-   🏭 Plant performance is highly concentrated, with one plant driving the majority of revenue.
-   👥 Sales are distributed across a wide range of customers, but top customers contribute a significant portion of revenue.

---

## 🎯 Model Strategy

### Approach

1.  **Unified Model**: A single, powerful model is trained on the most granular data (individual sales records).
2.  **Rich Feature Set**: The model's performance relies on a robust set of engineered features that capture temporal, seasonal, and entity-specific patterns.
3.  **Aggregation**: Predictions are made at the granular level and then aggregated to provide accurate plant-level and customer-level forecasts.

### Feature Engineering

-   **Temporal**: Year, Month, Week, Day of Year.
-   **Seasonal**: Sine/Cosine transformation of the month to handle cyclical patterns.
--   **Lag Features**: Sales from the previous 4, 8, and 12 weeks.
-   **Rolling Averages**: Smoothed sales trends over recent periods.
-   **Statistical**: Mean/Std/Count of sales per plant, customer, and product.

### Validation Strategy

-   **Chronological Split**: The data is split by a specific cutoff date, ensuring the model is trained on past data and validated on future data, which is critical for time-series problems.

---

## 📊 Success Metrics

**Primary KPI:**

-   **R-squared (R²)**: Aims for >80% to measure the proportion of sales variance captured by the model. **Achieved: 83.5%**.

**Secondary KPIs:**

-   **Root Mean Squared Error (RMSE)**: Measures the average magnitude of prediction errors.
-   **Mean Absolute Error (MAE)**: Measures the average absolute error.

---

## ✅ Project Status

**COMPLETED SUCCESSFULLY** ✅

-   All core project requirements were met and exceeded.
-   **83.5% prediction accuracy** was achieved, surpassing the 80% target.
-   A production-ready, single-notebook solution was delivered.
-   Comprehensive business analysis and actionable insights were generated.

---

**Last Updated:** August 15, 2025