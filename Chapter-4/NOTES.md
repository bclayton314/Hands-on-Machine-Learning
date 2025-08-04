# Training Models

## Linear Regression
Linear regression is a type of supervised machine-learning algorithm that learns from the labelled datasets and maps the data points with most optimized linear functions which can be used for prediction on new datasets. It assumes that there is a linear relationship between the input and output, meaning the output changes at a constant rate as the input changes. This relationship is represented by a straight line.  
y = mx + b  

Assumptions of the Linear Regression:  
1. Linearity: The relationship between inputs (X) and the output (Y) is a straight line.  
2. Independence of Errors: The errors in predictions should not affect each other.  
3. Constant Variance (Homoscedasticity): The errors should have equal spread across all values of the input. If the spread changes (like fans out or shrinks), it's called heteroscedasticity and it's a problem for the model.  
4. Normality of Errors: The errors should follow a normal (bell-shaped) distribution.  
5. No Multicollinearity(for multiple regression): Input variables shouldn’t be too closely related to each other.  
6. No Autocorrelation: Errors shouldn't show repeating patterns, especially in time-based data.  

Cost function for Linear Regression  
<img width="464" height="120" alt="image" src="https://github.com/user-attachments/assets/24503526-9a8d-441f-a648-4e90200992e7" />


Gradient Descent for Linear Regression  
Gradient descent is an optimization technique used to train a linear regression model by minimizing the prediction error. It works by starting with random model parameters and repeatedly adjusting them to reduce the difference between predicted and actual values.  

How it works:  
-Start with random values for slope and intercept.  
-Calculate the error between predicted and actual values.  
-Find how much each parameter contributes to the error (gradient).  
-Update the parameters in the direction that reduces the error.  
-Repeat until the error is as small as possible.  

### The Normal Equation


## Regularization
### Ridge and Lasso
Ridge and Lasso regression are techniques used to solve overfitting in linear regression models. They achieve this by adding a penalty term to the regression equation, which shrinks the regression coefficients towards zero, thus reducing model complexity and improving its ability to generalize to new data.


