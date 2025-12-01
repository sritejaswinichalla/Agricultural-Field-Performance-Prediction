# Agricultural Field Performance Prediction

## Project Overview

This project aims to predict whether an agricultural field is performing **high**, **moderately**, or **low** based on its efficiency in utilizing available resources, size, and other characteristics. The classification is not just about yield but about how well a field maximizes its potential given its constraints.

## Problem Statement

In agricultural systems, field performance isn't solely determined by absolute yield. A field might produce decent output but still be classified as "low performing" if it's not maximizing its potential due to factors like:
- Distance from market
- Inefficient resource utilization
- Suboptimal farming practices
- Poor logistics or infrastructure

## Goal

Develop a classifier that can predict agricultural field performance categories:
- **High performing**: Field is achieving or exceeding its potential
- **Moderately performing**: Field is within expected performance range with room for improvement  
- **Low performing**: Field is underperforming relative to its potential

## Evaluation Metric

The model is evaluated using **Macro F1-score**, which ensures balanced performance across all three classes and doesn't favor the majority class.

## Project Structure

```
├── cs24mtech14016_foml24_hackathon.ipynb    # Main analysis notebook
├── cs24mtech14016_foml24_hackathon_report.pdf    # Project report
└── README.md                                 # This file
```

## Methodology

The project follows a systematic approach:

1. **Exploratory Data Analysis (EDA)**
   - Data distribution analysis
   - Missing value assessment
   - Class balance evaluation
   - Feature correlation analysis

2. **Feature Engineering**
   - Temporal features (seasonal patterns, trends)
   - Spatial features (location-based characteristics)
   - Derived efficiency metrics
   - External data integration (weather, market data)

3. **Model Development**
   - Baseline models (Logistic Regression, Random Forest)
   - Advanced models (XGBoost, LightGBM, CatBoost)
   - Cross-validation with stratified folds
   - Hyperparameter optimization

4. **Model Validation**
   - Stratified K-fold cross-validation
   - Macro F1-score optimization
   - Class imbalance handling
   - Feature importance analysis

## Key Features

- **Resource Efficiency Metrics**: Yield per input ratios
- **Spatial Features**: Distance to markets, geographic characteristics
- **Temporal Patterns**: Seasonal trends, multi-year performance
- **Infrastructure**: Access to roads, irrigation, storage facilities
- **External Factors**: Weather patterns, soil quality indicators

## Requirements

- Python 3.8+
- pandas
- numpy
- scikit-learn
- xgboost/lightgbm
- matplotlib/seaborn
- jupyter

## Usage

1. Open `cs24mtech14016_foml24_hackathon.ipynb` in Jupyter
2. Run all cells sequentially
3. The notebook will generate predictions and evaluation metrics
4. Final model predictions are exported for submission

## Results

The project delivers:
- Comprehensive analysis of agricultural field performance factors
- Trained classification model optimized for macro F1-score
- Feature importance insights for agricultural efficiency
- Actionable recommendations for field improvement
