# 📈 Stock-Forecasting-Demo

### Machine Learning System for Forecasting the Next Trading Day of the S&P 500 ETF (SPY)

------------------------------------------------------------------------

## Overview

This repository contains my machine learning system for forecasting the
next trading day of the **S&P 500 ETF (SPY)**. The project compares
multiple forecasting models and progressively more advanced
feature-engineering techniques to develop a practical daily market
prediction system.

The system evaluates **AutoReg, ARIMA, SARIMAX, Logistic Regression,
L1-Regularized Logistic Regression (Lasso), L2-Regularized Logistic
Regression (Ridge), Elastic Net Logistic Regression, Decision Tree,
Random Forest, and XGBoost**, while systematically exploring different
approaches to feature engineering and model selection.

The full private system is designed to generate daily forecasts for SPY. This
public demo uses a fixed anonymized data snapshot. For
next-day market direction, the best models achieve approximately **57%
test accuracy**, about **2 percentage points higher** than the **Always
Up** baseline. The system also includes specialized downside-warning
models that identify significant market declines. Running multiple
models each trading day, the strongest downside-warning models detect
approximately **75%--80%** of the target large-down days while recording
all predictions for ongoing performance evaluation.

------------------------------------------------------------------------

# ⭐ Key Results

-   Compared **10** machine learning and time-series forecasting models.
-   Developed **5 model-building experiments** culminating in a forecasting
    system.
-   Achieved approximately **57%** next-day direction accuracy.
-   Improved approximately **2 percentage points** over the **Always
    Up** baseline.
-   Built specialized downside-warning models that detect approximately
    **75%--80%** of target large-down days.
-   Demonstrates SPY prediction generation and prediction-history tracking
    using the included data snapshot.

------------------------------------------------------------------------

# 📈 Model Development Timeline

``` text
Experiment 1
Time-Series Forecasting
        │
        ▼
Experiment 2
SPY Direction Prediction
        │
        ▼
Experiment 3
Multi-Market Features
        │
        ▼
Experiment 4
Compact Technical Features
        │
        ▼
Experiment 5
Extended Technical Features
        │
        ▼
Final Demo System
Forecasting Workflow
```

  ------------------------------------------------------------------------
  Stage            Objective                 Main Result
  ---------------- ------------------------- -----------------------------
  **Experiment 1** Forecast tomorrow's SPY   Traditional time-series
                   closing price using       models did not outperform a
                   AutoReg, ARIMA, and       persistence forecast.
                   SARIMAX                   

  **Experiment 2** Predict next-day SPY      Small Decision Trees
                   direction                 consistently outperformed
                                             more complex models, although
                                             overall gains remained
                                             modest.

  **Experiment 3** Add VIX, QQQ, TNX and     Additional market information
                   Bitcoin                   did not improve predictive
                                             performance.

  **Experiment 4** Compact                   Produced the strongest
                   technical-analysis        downside-warning models and
                   feature engineering       became the foundation of the
                                             final system.

  **Experiment 5** Extended feature          More features increased
                   engineering               complexity but did not
                                             improve predictive
                                             performance.

  **Final Demo     Forecasting workflow      Uses the strongest-performing
  System**                                   models and feature set
                                             discovered during development.
  ------------------------------------------------------------------------

------------------------------------------------------------------------

# 🤖 Models Evaluated

### Time-Series Models

-   AutoReg
-   ARIMA
-   SARIMAX

### Linear Classification Models

-   Logistic Regression
-   L1-Regularized Logistic Regression (Lasso)
-   L2-Regularized Logistic Regression (Ridge)
-   Elastic Net Logistic Regression

### Tree-Based Models

-   Decision Tree
-   Random Forest
-   XGBoost

------------------------------------------------------------------------

# 📂 Repository Structure

``` text
experiments/Stock-Forecasting-Experiment-1-Demo.ipynb
    Exact next-day SPY closing-price forecasting using classical time-series models.

experiments/Stock-Forecasting-Experiment-2-Demo.ipynb
    Next-day SPY direction prediction using technical indicators.

experiments/Stock-Forecasting-Experiment-3-Demo.ipynb
    Evaluating additional market information (VIX, QQQ, TNX, Bitcoin).

experiments/Stock-Forecasting-Experiment-4-Demo.ipynb
    Compact technical-analysis feature engineering and downside-warning models.

experiments/Stock-Forecasting-Experiment-5-Demo.ipynb
    Extended feature engineering and comparison with Experiment 4.

Stock-Forecasting-Final-Demo.ipynb
    Final forecasting demonstration with model evaluation, snapshot-based prediction, and prediction tracking.
```

------------------------------------------------------------------------

# 🚀 Quick Start

1.  Clone or download this repository.
2.  Install the required Python packages with `pip install -r requirements.txt`.
3.  Keep the included anonymized CSV files in the `data/` folder.
4.  Open the Final Demo from the repository root, or open an experiment
    from the `experiments/` folder.
5.  Run the selected notebook from top to bottom in JupyterLab or
    Jupyter Notebook.

The **Stock-Forecasting-Final-Demo.ipynb** notebook performs:

-   Anonymized feature-snapshot loading
-   Model training
-   Model evaluation
-   A demonstration prediction based on the included data snapshot
-   Prediction-history tracking

------------------------------------------------------------------------

# 🔒 Public Demo

This repository is intended as a portfolio demonstration.

The public version includes the complete modeling workflow after feature
generation, including feature loading, model training, evaluation, comparison,
prediction, interpretation, and prediction tracking.

To protect the privacy of the full project, the private feature-engineering
implementation and original feature definitions are intentionally omitted.
The public notebooks load anonymized precomputed feature matrices while
preserving the modeling and evaluation pipeline.

------------------------------------------------------------------------

# 📌 Broader ML Trading System

This SPY direction and downside-risk demo represents one component of a
broader machine-learning system that I am developing for stock trading. The
larger system uses specialized models to address different aspects of trading,
including market direction, return magnitude, volatility, market regimes,
relative performance, portfolio allocation, risk management, and trade
execution. My goal is to combine these focused models into a detailed,
risk-aware framework for making more informed trading decisions.

------------------------------------------------------------------------

# © Copyright

**Copyright © 2026 Tien Le. All rights reserved.**

This repository is provided for educational and portfolio demonstration
purposes. The proprietary feature-engineering methods and original
feature definitions are not included in this public release.
