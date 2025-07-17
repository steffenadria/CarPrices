# Car Price Prediction Using Regression and Machine Learning

This project explores a dataset of used car prices and applies several regression and machine learning models to predict vehicle prices based on features like horsepower, make, age, and fuel type.

## Dataset
Sourced from the UCI Automobile Dataset. It includes numerical and categorical variables. There were no missing values, and categorical variables were encoded using one-hot encoding.

## Models Compared
- Linear Regression (with Sequential Feature Selection and Ridge Regularization)
- Bayesian Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Support Vector Regression
- Neural Network with One Hidden Layer (PyTorch)

## Evaluation Metrics
- Root Mean Squared Error (RMSE)
- R-Squared Score
- AIC and BIC (for linear models)

## Best Model
**Random Forest Regressor** achieved the best performance:
- 13 trees
- Test RMSE: ~3063
- Most important predictor: **Horsepower**

## Key Takeaways
- Traditional linear regression performed well but was outpaced by ensemble and NN methods.
- Feature selection (via SFS and correlation analysis) significantly improved model clarity.
- PyTorch-based NN added extra validation and robustness.

## How to Run
Install dependencies:
```bash
pip install -r requirements.txt
```
Place `CarPrices.csv` in the same directory as the notebook, and run:
Then launch:
```bash
jupyter notebook
```

## Files
- `CarPricePrediction.ipynb` - Main notebook
- `requirements.txt` - Python package dependencies
- `README.md` - Project overview
- `CarPrices.csv` - Data set
- `LICENSE`

## License
MIT License
