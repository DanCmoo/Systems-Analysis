# Workshop 3 Report: Simulation of Solution for Backpack Price Prediction Models

## 📌 Overview
This repository contains the computational simulation of a robust system for backpack price prediction, developed as part of the **Systems Analysis & Design** course at Universidad Distrital FJDC. The project leverages the Kaggle Playground Series dataset (Season 5, Episode 2) to validate a machine learning pipeline with chaos theory integration.

## 🎯 Key Features
- **XGBoost-based prediction models** with/without material feature (Comparative analysis)
- **Automated data pipeline**: Preprocessing, outlier detection (Isolation Forest), and feature engineering
- **Chaos theory integration**: Sensitivity analysis via perturbations (±10%) and Partial Dependence Plots
- **Reproducible system design**: Docker, Dask, and Airflow-ready architecture

## 📊 Results Summary
| Model | RMSE Validation | MAE Validation | R² Validation |
|-------|-----------------|----------------|---------------|
| A (with material) | 38.72 | 30.15 | 0.82 |
| B (without material) | 39.50 | 31.10 | 0.80 |

**Key Findings**:
- Model A showed 7.5% higher sensitivity to weight capacity changes
- Identified 3,000 outliers (~1% of data) with chaotic response zones
- Material feature added predictive value but increased instability

## 🛠️ Implementation Highlights
```python
# Core Libraries
import pandas as pd
from sklearn.preprocessing import OrdinalEncoder
import xgboost as xgb

# Data Pipeline
!python scripts/preprocess.py --input-dir data/raw \
    --output-dir data/processed \
    --outname processed_data.csv
```
## 🔧 Setup
```python
pip install -r requirements.txt{
python scripts/preprocess.py --input-dir data/raw --output-dir data/processed
```

## 🌟 Next Steps
- Hyperparameter optimization
- Advanced chaos testing with Lyapunov exponents
- Docker containerization for deployment

