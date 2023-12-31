# Linear_Regression
## from sklearn.linear_model import LinearRegression -> [Scikit-Learn Linear Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)  

### Summary:

Linear Regression is a fundamental concept in machine learning. Linear regression is a statistical method used in machine learning and data analysis. It's used to predict the value of a dependent variable based on the value of one or more independent variables. The goal is to find the best linear relationship between these variables. Linear regression is used in various fields like economics for market forecasting, in biology for growth rate analysis, in finance for risk assessment, and many other areas where relationships between variables need to be understood and predictions are important.

Imagine you're trying to predict your final grade in a class based on the amount of time you spend studying. Linear Regression is a way of finding the relationship between two things: the cause (studying) and the effect (your grade). It's not perfect, real life is often more complicated, and many factors can affect your grade, not just study time. Linear Regression assumes a straight-line relationship, which might not always be the case. Linear Regression is like using a ruler to draw a straight line through a scatter of points on a graph. It helps us understand and predict how one thing affects another, a crucial skill in the world of data and machine learning!

Linear regression is an excellent starting point for statistical modeling and prediction, especially when you have linear relationships and relatively simpler datasets. However, its limitations in handling complex, non-linear relationships and sensitivity to outliers often necessitate the use of more sophisticated methods in real-world applications.



#### How Does it Work?

1. Drawing a Line Through Data: Think of each study session and the grade you got on a test afterward as a dot on a graph. Linear Regression tries to draw a straight line through these dots in a way that represents their relationship as accurately as possible.

2. The Best Fit Line: This line is called the "line of best fit". It shows the trend: as you increase your study time (moving right on the graph), your grades (going up on the graph) tend to improve.

3. Prediction: Once you have this line, you can use it to predict your grade. For example, if you study for 5 hours, you can see where that point is on the line and predict your grade.

<img width="645" alt="Screenshot 2023-12-30 at 8 47 36 AM" src="https://github.com/kasteway/Linear_Regression/assets/62068733/1f66935a-61cf-4672-931f-b44a7d22ffa7">


#### Why is it Important?

- Simplicity: Linear Regression is straightforward and easy to understand, making it a great starting point for learning about more complex machine learning models.
- Foundation: It forms the basis for understanding how we can use data to make predictions, which is a core aspect of machine learning.


---

#### Types of Linear Regression

##### Simple Linear Regression (Univariate Linear Regression):

- This involves two variables - one independent variable and one dependent variable. It tries to establish a linear relationship between these two.
- Example: Predicting house prices based on the size of the house (where house price is the dependent variable and house size is the independent variable).

##### Multiple Linear Regression:

- This involves more than one independent variable. It's used when the outcome depends on several factors.
- Example: Predicting a person's weight based on their height, age, and diet.

##### Polynomial Regression:

- A form of linear regression where the relationship between the independent variable and the dependent variable is modeled as an nth degree polynomial.
- Why It's 'Linear': Despite its name, polynomial regression is a form of linear regression because the coefficients are linear even if the variables are raised to a power.
- Example: Analyzing the growth rate of tissues or bacterial cultures, where the growth rate accelerates or decelerates over time.

---


#### Key Points
- Goal: To find the line (or plane, in the case of multiple variables) that best fits the data points.
- Use: It's widely used in forecasting, time series modeling, and finding the causal effect relationships between variables.
- Assumptions:
  1. Linear regression assumes a linear relationship between variables
  2. Constant variance in the residuals (homoscedasticity)
  3. Independence of residuals
  4. Normally distributed residuals


---


### Advantages & Disadvantages:

#### Advantages:

- Simplicity and Interpretability: Linear regression is straightforward to understand and interpret. The relationships between variables are represented with simple equations, making it easy to explain even to those without a strong statistical background.

- Efficient Computation: It requires less computational resources compared to more complex models, making it relatively fast and efficient.

- Predictive Power: Despite its simplicity, linear regression can provide reasonably accurate predictions in many cases, especially when the data has a linear relationship.

- Basis for Other Methods: It forms the foundation for understanding more complex models. Many advanced statistical techniques are extensions or modifications of linear regression.

- Continuous and Categorical Data: It can handle both types of data, either as dependent or independent variables.

- Useful for Trend Analysis: It's excellent for understanding trends and making forecasts, which is valuable in fields like finance and economics.


#### Disadvantages:

- Assumption of Linearity: Linear regression assumes a linear relationship between variables. This is often too simplistic for real-world data, which can be more complex and non-linear.

- Sensitive to Outliers: Linear regression models can be significantly impacted by outliers in the data, leading to inaccurate models and predictions.

- Homoscedasticity Requirement: It assumes that the residuals (differences between observed and predicted values) are constant across all levels of the independent variables. This isn't always the case in real data.

- Independence of Errors: The model assumes that the errors of the response variables are uncorrelated. This may not hold true, especially in time series data.

- Multicollinearity Issues: When independent variables are highly correlated, it can distort the importance of variables and make the model unstable.

- Limited to Linear Relationships: As the name implies, it can only model linear relationships. Many real-world scenarios involve non-linear dynamics that linear regression can't capture.

- Overfitting with Many Variables: In cases with many independent variables, the model might become overfit to the training data, leading to poor performance on unseen data.

---

## Algorithms used for optimizing the cost function:

1. Batch Gradient Descent - calculates the gradient of the cost function with respect to the parameters for the entire training dataset. As a result, it updates the model parameters only after it has computed the gradients for the entire dataset.
   -
   - Applications: Batch gradient descent is suitable for smaller datasets or when computational resources are sufficient to handle the entire dataset at once.
   - Challenges: It can be slow and computationally intensive, particularly with very large datasets. Also, it might not handle well with very large-scale machine learning problems where the dataset doesn't fit into memory.
   - 
2. Stochastic Gradient Descent (SGD) - updates parameters for each training example. It's faster but results in a more fluctuating convergence path.
   - 
3. Mini-batch Gradient Descent - This is a compromise between batch and stochastic gradient descent. It updates parameters after computing the gradient on small batches of the training data, offering a balance between speed and stability.
   -

---
## Tips:
- Gradient Descent -> is about iteratively adjusting the coefficients to minimize the difference between the predicted values and the actual values, as measured by a cost function like the MSE
- Learning Rate -> The learning rate determines the size of the steps we take towards the minimum. If it's too large, we might overshoot the minimum; if it's too small, the algorithm might take too long to converge.
- Convergence -> The process is repeated until the algorithm converges, meaning the change in the cost function is below a certain small threshold, or a maximum number of iterations is reached


---



## Resources:

- Wikipedia Simple Linear Regression Link - [Wikipedia Simple Linear Regression](https://en.wikipedia.org/wiki/Simple_linear_regression)
- Scikit-Learn Linear Regression - [Scikit-Learn Linear Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html) 

---
