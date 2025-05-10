# Backpack Price Prediction System - System Design

## Project Overview
This repository contains the system design and implementation for a machine learning model to predict backpack prices, building upon the analysis from [Workshop #1](https://github.com/DanCmoo/Systems-Analysis/blob/d320c17f7833124ebd685d5c2ce08b71752d3cde/Workshop_1/Workshop_1.pdf). The system addresses sensitivity and chaotic behavior in pricing patterns through robust architectural design.

## Key Features
- Dual XGBoost models (with/without material feature).
- Chaos theory implementation for outlier detection.
- Sensitivity analysis through partial dependence plots.
- Automated retraining mechanism.

## Development Process
### Phase 1: Review Analysis (Workshop #1)
[Refer to PDF report](https://github.com/DanCmoo/Systems-Analysis/blob/d320c17f7833124ebd685d5c2ce08b71752d3cde/Workshop_1/Workshop_1.pdf) for detailed findings from initial analysis that informed this design:
- Identified key price determinants: brand, material, size, compartments, etc.
- Detected high sensitivity to weight capacity and material changes.
- Observed chaotic pricing patterns in similar backpacks.

### Phase 2: Defyne System Requirements
For this phase, the functional and non-functional requirements approach was carried out.

### Phase 3: System Architecture
![Architecture Diagram](https://github.com/DanCmoo/Systems-Analysis/blob/01e0d184a657b408f2cc7eeab95b08cef25d2cf6/Workshop_2_Design/Architecture_Img.pdf)
)  
*Data flow and component interaction (see [section 3](#) in PDF report)*

### Phase 4: Sensitivity And Chaos
Substantiate the relationship between the proposed design and variables with high sensitivity or chaotic factors.

Key design decisions influenced by chaos theory:
- Isolation Forest for non-parametric outlier detection (±3σ thresholds)
- Observer pattern for automatic model retraining
- Uncertainty ranges instead of fixed price predictions

## Final Deliverable
1. [Final Report PDF](https://github.com/DanCmoo/Systems-Analysis/blob/1e76f63c385b3099bb8051ca4d8bc619566f90a4/Workshop_2_Design/Workshop_2.pdf) - Complete system documentation

## References
1. Kaggle Competition: [Playground Series - Season 5, Episode 2](https://www.kaggle.com/competitions/playground-series-s5e2)
2. XGBoost Documentation: [Regression with Chaotic Data](https://xgboost.readthedocs.io/)
