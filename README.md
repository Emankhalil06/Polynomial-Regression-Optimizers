# Polynomial Regression and Optimization Algorithms

## Project Overview
This project implements Linear Regression and Polynomial Regression to predict concrete compressive strength using five optimization algorithms implemented from scratch with NumPy.

## Dataset
The project uses the Concrete Compressive Strength dataset from Kaggle.

- Number of observations: 1,030
- Input features: 8
- Target variable: Concrete Compressive Strength (MPa)
- Missing values: None

## Algorithms Implemented
1. Gradient Descent with Momentum
2. Stochastic Gradient Descent (SGD)
3. Mini-Batch Gradient Descent
4. RMSProp
5. Adam

## Methodology
- Data preprocessing and missing-value checking.
- 80% training and 20% testing split.
- Feature scaling using StandardScaler.
- Polynomial feature generation with degree 2.
- Manual implementation of optimization algorithms using NumPy.
- Model evaluation using MSE, RMSE, MAE, and R².

## Results

Polynomial Regression achieved better performance than Linear Regression.

| Model | R² Score |
|---|---:|
| Linear Regression | 0.6281 |
| Polynomial Regression | 0.7863 |

RMSProp achieved the best test performance among the five optimization algorithms, with an R² score of 0.7863.

## Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Kaggle Notebooks

## Project Structure
- `polynomial-regression-optimizers.ipynb`: Complete project implementation, experiments, evaluation, and visualizations.

## References
- [Concrete Compressive Strength Dataset](https://www.kaggle.com/datasets/niteshyadav3103/concrete-compressive-strength)
- [NumPy Documentation](https://numpy.org/doc/)
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)
