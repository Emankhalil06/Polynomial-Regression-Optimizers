# Polynomial Regression and Optimization Algorithms

## Project Overview

This project implements Polynomial Regression to predict concrete compressive strength using five optimization algorithms implemented from scratch with NumPy.

The main objective is to study and compare the performance of different optimization algorithms when training a Polynomial Regression model.

## Dataset

The project uses the Concrete Compressive Strength dataset from Kaggle.

- Number of observations: 1,030
- Input features: 8
- Target variable: Concrete Compressive Strength (MPa)
- Missing values: None

## Algorithms Implemented

The following optimization algorithms were implemented manually using NumPy:

1. Gradient Descent with Momentum
2. Stochastic Gradient Descent (SGD)
3. Mini-Batch Gradient Descent
4. RMSProp
5. Adam

## Methodology

- Dataset loading and exploration.
- Data preprocessing and missing-value checking.
- 80% training and 20% testing split.
- Feature scaling using StandardScaler.
- Polynomial feature generation with degree 2.
- Manual implementation of optimization algorithms using NumPy.
- Model training and loss visualization.
- Model evaluation using MSE, RMSE, MAE, and R².

## Results

The Polynomial Regression models were evaluated using the same dataset split and preprocessing approach.

| Optimizer | MSE | RMSE | MAE | R² Score |
|---|---:|---:|---:|---:|
| GD with Momentum | 55.1723 | 7.4278 | 5.9650 | 0.7859 |
| SGD | 57.9620 | 7.6133 | 6.1035 | 0.7751 |
| Mini-Batch GD | 55.8404 | 7.4726 | 6.0009 | 0.7833 |
| RMSProp | 55.0620 | 7.4204 | 5.9621 | 0.7863 |
| Adam | 62.9763 | 7.9358 | 6.4454 | 0.7556 |

RMSProp achieved the best test performance among the five optimization algorithms, with an R² score of 0.7863.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Kaggle Notebooks

## Project Structure

- `01-gd-momentum.ipynb`: Gradient Descent with Momentum implementation.
- `02-sgd.ipynb`: Stochastic Gradient Descent implementation.
- `03-mini-batch-gd.ipynb`: Mini-Batch Gradient Descent implementation.
- `04-rmsprop.ipynb`: RMSProp implementation.
- `05-adam.ipynb`: Adam implementation.
- `Concrete Compressive Strength.csv`: Dataset used in the project.
- `polynomial-regression-optimizers.ipynb`: Original combined project implementation.
- `README.md`: Project documentation.

## References

- [Concrete Compressive Strength Dataset - Kaggle](https://www.kaggle.com/datasets/niteshyadav3103/concrete-compressive-strength)
- [NumPy Documentation](https://numpy.org/doc/)
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)
