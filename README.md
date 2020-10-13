# Model Selection on Auto Data

Code Written in R using RStudio Notebook. Open the R Markdown file [here](https://github.com/sshreyas999/Model-Selection-on-Auto-Data/blob/main/Model%20Selection%20on%20Auto%20Data.Rmd) for code and commentary.


## Objective  
Our goal is to build a model that can predict `mpg`. We want to be able to predict the mileage of a vehicle from other attributes.

## Dataset
The `Auto` dataset is available in the `ISLR` package. The dataset contains 392 observations with 9 attributes for each observation. The attributes are briefly described below:

1. mpg - miles per gallon
2. cylinders - Number of cylinders between 4 and 8
3. displacement - Engine displacement (cu. inches)
4. horsepower - Engine horsepower
5. weight - Vehicle weight (lbs.)
6. acceleration - Time to accelerate from 0 to 60 mph (sec.)
7. year - Model year (modulo 100)
8. origin - Origin of car (1. American, 2. European, 3. Japanese)
9. name - Vehicle name

We ignore the **name** attribute as it is too varied to include in the model. We use all the data to train the model, and compute test error through cross validation.

## Outline  
### Exploratory Analysis of Dataset
See what variables are useful in predicting the outcome. Perform transformations as required.
### Model Fitting
Fit the model using:
#### Standard Least Squares  
#### Best-subset selection
#### Ridge regression
#### Lasso regularization
#### Principal Component Regression (PCR)
#### Partial Least Squares (PLS)
### Comparision & Conclusions
Compare coefficients, MSE, and find the best model.

## Conclusion
The best model was achived through Partial Least Squares (PLS). It gave us the lowest MSE - 8.677.
