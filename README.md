# California Housing Price Prediction

This project applies various regression techniques to predict median house prices in California using the California Housing dataset from the `sklearn` library. The goal is to evaluate and compare the performance of different regression algorithms.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Methodology](#methodology)
6. [Results](#results)
7. [Conclusion](#conclusion)
8. [License](#license)
9. [Acknowledgments](#acknowledgments)
10. [Contact](#contact)

---

## Project Overview

The objective of this project is to evaluate regression techniques in supervised learning by applying them to the California Housing dataset. The key steps include:
1. **Loading and Preprocessing**: Load the dataset, handle missing values (if any), and perform feature scaling.
2. **Regression Algorithm Implementation**: Implement and train five regression models:
   - Linear Regression
   - Decision Tree Regressor
   - Random Forest Regressor
   - Gradient Boosting Regressor
   - Support Vector Regressor (SVR)
3. **Model Evaluation and Comparison**: Evaluate models using Mean Squared Error (MSE), Mean Absolute Error (MAE), and R-squared (R²) metrics. Compare the results to identify the best and worst-performing models.

---

## Dataset

The California Housing dataset contains information about housing in California, including features such as:
- **MedInc**: Median income in the area
- **HouseAge**: Median house age in the area
- **AveRooms**: Average number of rooms per household
- **AveBedrms**: Average number of bedrooms per household
- **Population**: Total population in the area
- **AveOccup**: Average number of household members
- **Latitude**: Latitude of the area
- **Longitude**: Longitude of the area

The target variable is **MedPrice**, which represents the median house price for households in the area.

### Dataset Characteristics
- Number of instances: 20,640
- Number of features: 8
- Target variable: Continuous (median house price)
- Missing values: None

---

## Installation

### Prerequisites
- Python 3.7 or higher
- pip (Python package installer)

### Steps to Set Up the Project

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/musabbirkm/CaliforniaHousingRegressionAnalysis.git
   cd CaliforniaHousingRegressionAnalysis
