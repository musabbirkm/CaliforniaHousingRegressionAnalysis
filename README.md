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

## Methodology

### Preprocessing

#### Feature Scaling:
- Features are standardized using **StandardScaler** to ensure all features have a mean of 0 and a standard deviation of 1.
- This is necessary for algorithms like **Linear Regression** and **SVR**, which are sensitive to the scale of input features.

#### Train-Test Split:
- The dataset is split into **training (80%)** and **testing (20%)** sets to evaluate model performance on unseen data.

### Regression Algorithms

1. **Linear Regression**:
   - Models a linear relationship between features and the target.
   - Suitable as a baseline model.

2. **Decision Tree Regressor**:
   - Splits data into subsets based on feature thresholds.
   - Captures non-linear relationships but is prone to overfitting.

3. **Random Forest Regressor**:
   - Ensemble of decision trees to reduce overfitting.
   - Handles non-linear relationships and feature interactions effectively.

4. **Gradient Boosting Regressor**:
   - Sequentially builds trees to correct errors from previous trees.
   - Achieves high accuracy by focusing on hard-to-predict instances.

5. **Support Vector Regressor (SVR)**:
   - Uses a kernel trick to model non-linear relationships.
   - Suitable for small to medium-sized datasets but requires careful tuning.

### Evaluation Metrics

- **Mean Squared Error (MSE)**: Measures the average squared difference between predicted and actual values. Lower values indicate better performance.
- **Mean Absolute Error (MAE)**: Measures the average absolute difference between predicted and actual values. Less sensitive to outliers compared to MSE.
- **R-squared (R²)**: Represents the proportion of variance in the target variable explained by the model. Higher values indicate better performance.

## Results

### Model Comparison

| Model                    | MSE    | MAE    | R²     |
|--------------------------|--------|--------|--------|
| Gradient Boosting         | 0.2950 | 0.3339 | 0.7887 |
| Random Forest             | 0.3254 | 0.3507 | 0.7666 |
| Decision Tree             | 0.4836 | 0.4656 | 0.6532 |
| Linear Regression         | 0.5552 | 0.5332 | 0.6016 |
| Support Vector Regressor  | 0.6285 | 0.5469 | 0.5503 |

### Best Model
- **Gradient Boosting Regressor** achieved the lowest **MSE (0.2950)** and highest **R² (0.7887)**.

### Worst Model
- **Support Vector Regressor** had the highest **MSE (0.6285)** and lowest **R² (0.5503)**.

## Conclusion
- **Gradient Boosting Regressor** performed the best due to its ability to model complex relationships and correct errors iteratively.
- **Support Vector Regressor** performed the worst, likely due to the dataset's size and the need for hyperparameter tuning.
- Tree-based models (**Random Forest** and **Gradient Boosting**) outperformed linear models, indicating that non-linear relationships are present in the data.



## Acknowledgments

- **Dataset**: California Housing Dataset from sklearn.
- **Libraries**: numpy, pandas, scikit-learn, matplotlib, and jupyter.
- **Inspiration**: This project was inspired by the need to evaluate and compare regression techniques for real-world datasets.

## Contact

- **Name**: Musabbir Km
- **Email**: musabbirmushu@gmail.com
- **GitHub**: [musabbirkm](https://github.com/musabbirkm)
- **LinkedIn**: [Musabbir Km](https://www.linkedin.com/in/musabbir-km)
## Installation

### Prerequisites
- Python 3.7 or higher
- pip (Python package installer)

### Steps to Set Up the Project

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/musabbirkm/CaliforniaHousingRegressionAnalysis.git
   cd CaliforniaHousingRegressionAnalysis
   pip install -r requirements.txt
