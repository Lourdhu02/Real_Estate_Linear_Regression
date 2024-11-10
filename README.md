
# Real Estate House Price Prediction

This project aims to predict house prices in a specific area using linear regression. By analyzing factors such as house age, proximity to public transportation, and the number of nearby convenience stores, the model predicts the price per unit area.

## Dataset

The dataset contains 414 entries with the following columns:

- `transaction date`: Date of the transaction.
- `house age`: Age of the house in years.
- `distance to the nearest MRT station`: Distance from the house to the nearest MRT station.
- `number of convenience stores`: Number of convenience stores within the vicinity.
- `latitude`: Latitude of the house.
- `longitude`: Longitude of the house.
- `house price of unit area`: Price per unit area.

## Project Overview

This project utilizes Python libraries, including `pandas`, `scikit-learn`, `seaborn`, and `matplotlib`, to perform data analysis and visualize correlations between features. Key steps include:

1. **Data Preprocessing**:
   - Loaded and inspected the dataset.
   - Dropped unnecessary columns and renamed columns for clarity.
   - Checked and handled any missing values (none in this dataset).

2. **Exploratory Data Analysis (EDA)**:
   - Correlation Heatmap: Visualizes correlations between features.
   - Histograms and Box Plots: Explore distribution of each feature.
   - Regression Plots: Shows the relationship between house prices and various features.

3. **Model Training**:
   - Performed a train-test split on the dataset.
   - Trained a Linear Regression model using scikit-learn.
   - Evaluated the model using Mean Squared Error (MSE) and R-squared values.

4. **Model Evaluation**:
   - Initial Model:
     - **Mean Squared Error**: 54.58
     - **R-squared**: 0.675
   - Improved Model (after removing outliers):
     - **Mean Squared Error**: 45.42
     - **R-squared**: 0.701

5. **Visualization of Results**:
   - Scatter plot of actual vs. predicted values to assess the model's performance visually.
   - Residual plot to observe the distribution of errors.

## Key Findings

- The model explains approximately 70% of the variance in house prices, indicating a reasonably good fit.
- Removing outliers slightly improved model performance.

## Future Improvements

- Experiment with other algorithms (e.g., Random Forest, Support Vector Machine) for potentially better predictions.
- Implement feature engineering to explore additional predictors that may impact house prices.

## Getting Started

### Prerequisites

- Python 3.8+
- Required libraries:
  ```bash
  pip install numpy pandas scikit-learn matplotlib seaborn
  ```

### Running the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/Lourdhu02/real-estate-house-price-prediction.git
   ```
2. Run the Jupyter Notebook or Python script containing the analysis.

Feel free to reach out for any questions or contributions!
```

This README provides a concise overview of the project and instructions for running it. Let me know if you need more adjustments!
