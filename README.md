# 🌲 Forest Health Analysis: Tree Height Prediction

This project performs an exploratory analysis and applies **Linear Regression** models to predict tree height (`Tree_Height`) based on environmental, geographic, and soil composition variables.

## 📊 Project Overview
The main objective is to understand how factors such as altitude, terrain slope, and soil nutrients (Nitrogen and Phosphorus) influence the vertical growth of trees in different sampling plots.

## 🛠️ Technologies Used
* **Python 3.13**
* **Pandas & NumPy:** Data manipulation and cleaning.

* **Matplotlib & Seaborn:** Statistical visualization and correlation matrices.

* **Scikit-Learn:** Data splitting (train_test_split) and implementation of the Linear Regression model.

## 📂 Dataset Structure
The dataset `forest_health_data.csv` contains 1000 records with the following main variables:
* **DBH (Diameter at Breast Height):** Tree diameter at breast height.

* **Slope & Elevation:** Slope and altitude of the terrain.

* **Soil Nutrients:** Nitrogen (TN/AN) and Phosphorus (TP/AP) content in the soil.

* **Target (Tree_Height):** Total tree height in meters.

## 📈 Modeling Results

### Correlation Matrix
The initial analysis via Heatmap allows identifying the strength of the relationship between the independent variables and the target.

### Model Performance
Currently, the simple linear regression model presented the following indicators:
* **R² (Coefficient of Determination):** -0.01 (Indicates that the current model does not explain the variability of the data better than the mean).

* **MSE (Mean Squared Error):** 63.47.

### Importance of Variables
Through the model coefficients, we identified which factors have the greatest weight (positive or negative) in the height estimate, such as **DBH** and **Elevation**.

## 🚀 How to Run

1. Install the dependencies:

``bash
pip install pandas matplotlib seaborn scikit-learn
