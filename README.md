# StockPredictor: Amazon Stock Price Prediction using Linear Regression

## Project Overview
StockPredictor is a machine learning project aimed at predicting Amazon's stock price using linear regression. The dataset consists of various commodity prices and trading volumes, such as Natural Gas, Crude Oil, Bitcoin, S&P 500, and more. The goal is to leverage historical market data to forecast Amazon’s stock price based on these key features.

This project covers all aspects of the machine learning pipeline, including data exploration, feature engineering, model development, validation, and testing.


## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Dataset
The dataset contains the following columns:
- **Date**
- **Natural_Gas_Price**, **Natural_Gas_Vol.**
- **Crude_oil_Price**, **Crude_oil_Vol.**
- **Bitcoin_Price**, **Bitcoin_Vol.**
- **S&P_500_Price**, **Nasdaq_100_Price**, **Nasdaq_100_Vol.**
- **Apple_Price**, **Apple_Vol.**
- **Tesla_Price**, **Tesla_Vol.**
- **Microsoft_Price**, **Microsoft_Vol.**
- **Amazon_Price**, **Amazon_Vol.** (Target Variable)
- And many more.
  
## Methodology
### Data Preprocessing
Missing Values: Filled missing values with the mean of their respective columns.
Feature Scaling: Standardized the dataset using StandardScaler for uniformity across features.
Correlation Analysis: Conducted a correlation analysis using a matrix to determine feature importance and multicollinearity.
### Model Development
Linear Regression: Trained a linear regression model to predict Amazon's stock price.
Train-Test Split: Split the dataset into an 80-20 ratio for training and testing.
Metrics Used: Evaluated the model using Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).
### Model Validation
Cross-Validation: Performed 5-fold cross-validation to ensure model generalization.
Feature Importance: Analyzed the model's coefficients to assess the importance of each feature.
Results
The linear regression model performed with reasonable accuracy:

###### Mean Absolute Error (MAE): 5.094387862758271
###### Mean Squared Error (MSE): 42.55004809953231
###### Root Mean Squared Error (RMSE): 6.523039789816732


### Challenges Faced
-**Multicollinearity:** Highly correlated features, such as Nasdaq 100 and S&P 500 prices, posed a challenge in model interpretability and performance.

-**Overfitting:** Cross-validation helped in preventing overfitting, ensuring the model performs well on unseen data.
