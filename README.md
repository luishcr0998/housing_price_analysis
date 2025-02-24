# 🏠 Housing Prices Analysis: Short-term Forecasting Model

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.7+-blue.svg" alt="Python Version">
  <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License">
  <img src="https://img.shields.io/badge/Status-Active-success.svg" alt="Status">
</p>

## 📋 Table of Contents
- [Overview](#overview)
- [Key Features](#key-features)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Project Structure](#project-structure)
- [Visualizations](#visualizations)
- [Results and Insights](#results-and-insights)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Future Work](#future-work)
- [License](#license)

## 🔍 Overview

This project develops a sophisticated short-term prediction model for residential property values using Zillow Group's comprehensive real estate data. The analysis captures representative dwelling costs and market fluctuations across various locations and property types.

While the primary focus is on the Boston, MA real estate market, the methodology is designed to be adaptable to other metropolitan areas, providing valuable insights for homebuyers, investors, and real estate professionals.

## ✨ Key Features

- Advanced time series forecasting for housing prices
- Two-component additive model combining non-stationary and stationary elements
- Comprehensive exploratory data analysis with statistical validation
- Temporal decomposition of price trends
- Robust model evaluation using cross-validation techniques
- Interactive visualizations of market trends and predictions

## 📊 Dataset

The analysis leverages Zillow's housing data, which includes:
- Historical median home values
- Time-series data across multiple geographic regions
- Property-type segmentation
- Monthly price indices

The Boston metropolitan area serves as the primary case study, with data spanning multiple years to capture both short-term fluctuations and longer-term trends.

## 🔬 Methodology

The project implements an innovative additive forecasting model in the form:

```
X̂ₜ = ŷₜ + ARₜ
```

Where:
- **X̂ₜ**: Estimated housing prices in Boston
- **ŷₜ**: Non-stationary component (Hankel-based unstructured model)
- **ARₜ**: Stationary component (autoregressive model)

### Modeling Workflow

1. **📈 Exploratory Data Analysis (EDA)**
   - Rigorous data verification and preparation
   - Comprehensive descriptive statistical analysis
   - Advanced outlier detection and treatment
   - Multi-dimensional visualizations
   - Statistical tests for normality and stationarity
   - Correlation matrix analysis
   - Temporal pattern identification

2. **🧮 Two-Stage Modeling Approach**
   - **Stage 1**: Hankel-based unstructured model for capturing non-stationary trends
     - Matrix formulation using Singular Value Decomposition (SVD)
     - Optimal rank selection through cross-validation
   - **Stage 2**: Residual modeling with autoregressive techniques
     - Order selection using information criteria (AIC/BIC)
     - Parameter estimation via maximum likelihood

3. **📏 Performance Evaluation Framework**
   - Mean squared error and mean absolute percentage error metrics
   - Time series-specific cross-validation methodology
   - Rolling window predictions for stability assessment
   - Comparison with benchmark models (ARIMA, Prophet)

## 📁 Project Structure

The analysis is contained in a well-documented Jupyter notebook (`housing_prices_analysis.ipynb`) that guides users through each step of the modeling process with detailed explanations and visualizations.

## 📊 Visualizations

The project includes numerous interactive and static visualizations:
- Price trend heatmaps across geographic regions
- Temporal decomposition plots (trend, seasonality, residuals)
- Prediction interval charts
- Residual diagnostic plots
- Model performance comparisons
- Feature importance visualizations

## 🔍 Results and Insights

The additive forecasting model provides:
- Accurate short-term price predictions with quantified uncertainty
- Identification of key market turning points
- Seasonal patterns in the Boston housing market
- Comparative analysis with traditional forecasting methods
- Actionable insights for market timing decisions

## 💻 Technologies Used

- **Data Processing**: pandas (1.3+), numpy (1.20+)
- **Statistical Analysis**: scipy (1.7+), statsmodels (0.13+)
- **Machine Learning**: scikit-learn (0.24+)
- **Visualization**: matplotlib (3.4+), seaborn (0.11+), plotly (5.0+)
- **Development Environment**: Jupyter/IPython (7.0+)

## 🚀 Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/housing-prices-analysis.git
cd housing-prices-analysis

# Create a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

## 📖 Usage

1. Ensure all dependencies are installed
2. Open the Jupyter notebook:
   ```bash
   jupyter notebook housing_prices_analysis.ipynb
   ```
3. Run the cells sequentially to reproduce the analysis
4. Modify parameters as needed for different scenarios or geographic regions

## 🔮 Future Work

- Extension to additional metropolitan areas for comparative analysis
- Integration of external economic indicators (interest rates, employment data)
- Implementation of deep learning approaches (LSTM, Transformer models)
- Development of a web-based interactive dashboard
- Incorporation of geospatial analysis for neighborhood-level predictions
- Real-time data integration for continuously updated forecasts

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

<p align="center">
  <i>For questions or collaborations, please open an issue or contact the repository owner.</i>
</p>

