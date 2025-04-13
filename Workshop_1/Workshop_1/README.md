# Backpack Price Prediction - Systemic Analysis Report

This folder contains the report and resources for the project: **Predicting the Price of Backpacks**, aiming to predict backpack prices based on various features using systemic thinking and machine learning techniques.

## 📄 Overview

The main objective was to design and implement a solution capable of predicting backpack prices based on a dataset provided by Kaggle. The dataset included 300,000 records and 11 features describing backpacks (e.g., brand, material, size, compartments, etc.).

The solution was built around the following steps:

1. **Data Preprocessing**  
   Using `pandas` and `numpy`, we explored the dataset, checked for unique values, handled inconsistencies, and prepared the data for modeling.

2. **Systemic Analysis**  
   We applied principles from systems engineering (homeostasis, adaptability, resilience, and emergence) to better understand the dynamics of the backpack market. This helped us model complex interactions between features such as material quality, size, and external market influences.

3. **Modeling**  
   - **Linear Regression** was used to explore basic relationships.
   - **Multiple Linear Regression** (via `scikit-learn`) was implemented to predict backpack prices based on the selected features.

4. **Model Evaluation**  
   We tested how sensitive the model was to small changes in feature values and examined edge cases to understand where the model might fail due to chaos or randomness in real-world data.

## 🧠 Key Insights

- **Features like brand, weight capacity, and waterproofing significantly influenced price.**
- **Small changes in attributes could cause drastic variations in predicted price.**
- **Certain external factors (e.g., marketing, seasonal trends) introduced non-linear effects beyond the scope of the model.**

## 📈 Tools Used

- Python
- Pandas & NumPy
- Scikit-learn
- Matplotlib / Seaborn (optional for visualizations)

## 📊 Dataset

- Source: Kaggle Playground Series - Season 5, Episode 2  
  [Kaggle Dataset](https://www.kaggle.com/competitions/playground-series-s5e2)

## 📚 Authors

- Daniel Esteban Camacho Ospina  
- Edgar Julian Roldan Rojas  
- Juan Esteban Rodriguez Camacho

All affiliated with Universidad Distrital Francisco José de Caldas.

## 📎 Related Files

- `Workshop_1.pdf`: Full report detailing the methodology and results.
- `code/`: Folder containing the scripts used for analysis and modeling.
- `figures/`: Visuals referenced in the report.

## Notebook

- Here you can find the use of code related to the system analysis:
- 👉 [Open in Deepnote](https://deepnote.com/workspace/Taller-acb46dcd-7c34-4618-9533-c5b95652cd77/project/analisis-7f8d2950-8be9-411c-b60d-045fbd99c90b/notebook/Notebook-1-70e476adb7da443384987786b77f0e17?utm_source=share-modal&utm_medium=product-shared-content&utm_campaign=notebook&utm_content=7f8d2950-8be9-411c-b60d-045fbd99c90b)

This notebook contains all code used for data preprocessing, feature analysis, model training, and evaluation.
