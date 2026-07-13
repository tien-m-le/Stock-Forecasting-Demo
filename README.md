# 📈 Stock-Forecasting-Demo

### Machine Learning System for Forecasting the Next Trading Day of the S&P 500 ETF (SPY)

------------------------------------------------------------------------

## Overview

This repository contains my machine learning system for forecasting the
next trading day of the **S&P 500 ETF (SPY)**. The project compares
multiple forecasting models and progressively more advanced
feature-engineering techniques to develop a practical daily market
prediction system.

The research evaluates **AutoReg, ARIMA, SARIMAX, Logistic Regression,
L1-Regularized Logistic Regression (Lasso), L2-Regularized Logistic
Regression (Ridge), Elastic Net Logistic Regression, Decision Tree,
Random Forest, and XGBoost**, while systematically exploring different
approaches to feature engineering and model selection.

The final production system generates live daily forecasts for SPY. For
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
-   Developed **5 research experiments** culminating in a production
    forecasting system.
-   Achieved approximately **57%** next-day direction accuracy.
-   Improved approximately **2 percentage points** over the **Always
    Up** baseline.
-   Built specialized downside-warning models that detect approximately
    **75%--80%** of target large-down days.
-   Generates **live daily SPY predictions** and automatically records
    prediction history.

------------------------------------------------------------------------

# 📈 Research Timeline

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
Final Production System
Live Daily Forecasting
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

  **Final          Live daily forecasting    Uses the strongest-performing
  Production                                 models and feature set
  System**                                   discovered during the
                                             research process.
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
Experiment-1-Demo.ipynb
    Exact next-day SPY closing-price forecasting using classical time-series models.

Experiment-2-Demo.ipynb
    Next-day SPY direction prediction using technical indicators.

Experiment-3-Demo.ipynb
    Evaluating additional market information (VIX, QQQ, TNX, Bitcoin).

Experiment-4-Demo.ipynb
    Compact technical-analysis feature engineering and downside-warning models.

Experiment-5-Demo.ipynb
    Extended feature engineering and comparison with Experiment 4.

Stock-Forecasting-Final-Demo.ipynb
    Final production forecasting system with live prediction and prediction tracking.
```

------------------------------------------------------------------------

# 🚀 Quick Start

1.  Clone or download this repository.
2.  Install the required Python packages.
3.  Place all files in the same directory.
4.  Open any notebook in JupyterLab or Jupyter Notebook.
5.  Run the notebook from top to bottom.

The **Stock-Forecasting-Final-Demo.ipynb** notebook performs:

-   Live SPY data download
-   Feature loading
-   Model training
-   Model evaluation
-   Current market prediction
-   Prediction history update

------------------------------------------------------------------------

# 🔒 Public Demo

This repository is intended as a portfolio demonstration.

The complete machine learning workflow---including data preparation,
model training, evaluation, comparison, live prediction, and prediction
tracking---is included.

To protect the original research, the proprietary feature-engineering
implementation and original feature definitions are intentionally
omitted. The public notebooks load anonymous precomputed feature
matrices while preserving the complete modeling pipeline.

------------------------------------------------------------------------

# 📌 Future Work

Potential future improvements include:

-   Automated feature selection
-   Additional macroeconomic indicators
-   Deep learning architectures
-   Reinforcement learning for trading strategies
-   Ensemble forecasting systems
-   Walk-forward retraining and automated deployment

------------------------------------------------------------------------

# © Copyright

**Copyright © 2026 Tien Le. All rights reserved.**

This repository is provided for educational and portfolio demonstration
purposes. The proprietary feature-engineering methods and original
feature definitions are not included in this public release.
