# Regularized-Regression_Predicting-Housing-Price
A machine learning model has three error sources: bias, variance, and irreducible error (inherent noise). One solution to minimize these errors is to reduce variance, such as using a simpler model. An example is regularized model. In linear regression, regularization is a process of making the model more regular or simpler by shrinking the model coefficient to be closer to zero or absolute, ultimately to address overfitting. 

In this project, I take the dataset of predicting the house pricing. The meaning of each column is explained in the project.

Below is the modeling flow to conduct regularized regression:
1. Split Data: train - validate - test
2. Correlation plot on training data
3. Fit the model on training data
4. Choose the best lambda from the validation test
5. Evaluate the model on test data using MAE, MAPE, and RMSE

Conclusions:
1. Best lambda from the validation set:

Using Ridge regressions,

- lambda = 0.01. For example, an increase of 1 point in zn, while the other features are kept fixed, is associated with an increase of 3.796482e-02 point in medv.

Using LASSO regressions,

- lambda = 0.01. For example, an increase of 1 point in zn, while the other features are kept fixed, is associated with an increase of 3.673332e-02 point in medv.

2. Best model on the test data:

Using Ridge regressions,

- The standard deviation of prediction errors (RMSE) to the regression line is 6.820639
- 3.896186 in MAE is equivalent to 17.1% (MAPE) deviation relative to the true housing price

Using LASSO regressions,  
- The standard deviation of prediction errors (RMSE) to the regression line is 6.823445
- 3.888415 in MAE is equivalent to 17.07% (MAPE) deviation relative to the true housing price
