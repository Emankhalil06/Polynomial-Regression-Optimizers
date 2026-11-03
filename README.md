# Polynomial Regression and Optimization Algorithms

## Project Overview

This project implements Linear Regression and Polynomial Regression to predict concrete compressive strength using five optimization algorithms implemented from scratch with NumPy.

The project focuses on understanding and comparing different optimization techniques, including Momentum-based updates.

## Dataset

The project uses the **Concrete Compressive Strength Dataset** from Kaggle.

- Number of observations: 1,030
- Input features: 8
- Target variable: Concrete Compressive Strength (MPa)
- Missing values: None

## Optimization Algorithms

Five optimization algorithms were implemented using NumPy:

1. **Gradient Descent with Momentum (GD)**
2. **Stochastic Gradient Descent with Momentum (SGD)**
3. **Mini-Batch Gradient Descent with Momentum**
4. **RMSProp with Momentum**
5. **Adam with Momentum**

### Momentum Implementation

Momentum was incorporated into the optimization algorithms to use information from previous gradients during parameter updates.

- GD: Uses the Momentum technique directly.
- SGD: Uses velocity terms to incorporate previous gradients.
- Mini-Batch GD: Applies Momentum to mini-batch gradient updates.
- RMSProp: Combines adaptive gradient scaling with Momentum.
- Adam: Uses the first moment (Beta1) as an exponential moving average of gradients, representing its momentum mechanism.

## Methodology

The project follows these steps:

1. Dataset loading and exploration.
2. Checking for missing values.
3. Splitting the dataset into 80% training and 20% testing.
4. Feature scaling using StandardScaler.
5. Generating polynomial features of degree 2.
6. Implementing the five optimizers manually using NumPy.
7. Training and monitoring model performance.
8. Evaluating the models using:
   - Mean Squared Error (MSE)
   - Root Mean Squared Error (RMSE)
   - Mean Absolute Error (MAE)
   - R² Score
9. Visualizing training loss and actual versus predicted values.

## Experimental Results

The following table presents the evaluation results obtained on the test dataset after incorporating Momentum.

| Optimizer | MSE | RMSE | MAE | R² Score |
|---|---:|---:|---:|---:|
| GD with Momentum | 55.1723 | 7.4278 | 5.9650 | 0.7859 |
| SGD with Momentum | 58.2073 | 7.6294 | 6.0610 | 0.7741 |
| Mini-Batch GD with Momentum | 55.4566 | 7.4469 | 5.9665 | 0.7848 |
| RMSProp with Momentum | 55.6280 | 7.4584 | 5.9721 | 0.7841 |
| Adam with Momentum | 62.9763 | 7.9358 | 6.4454 | 0.7556 |

### Results Analysis

Based on the test results, Gradient Descent with Momentum achieved the highest R² score of 0.7859 among the five implementations.

Mini-Batch GD and RMSProp with Momentum also achieved competitive results.

Adam achieved a lower R² score on this dataset with the selected hyperparameters.

These results demonstrate that optimizer performance depends on the optimization method and its hyperparameter settings.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Kaggle Notebooks
- GitHub

## Project Structure

```text
Polynomial-Regression-Optimizers/
│
├── 01-gd-momentum.ipynb
├── 02-sgd.ipynb
├── 03-mini-batch-gd.ipynb
├── 04-rmsprop.ipynb
├── 05-adam.ipynb
│
├── Concrete Compressive Strength.csv
└── README.md
```

## References

- Concrete Compressive Strength Dataset – Kaggle
- NumPy Documentation
- Pandas Documentation
- Scikit-learn Documentation

## Author

**Eman Khalil**

Data Science and Artificial Intelligence Student

Al al-Bayt University
