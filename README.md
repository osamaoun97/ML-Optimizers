# ML Optimizers

Linear regression is a commonly used machine learning algorithm that involves
finding a linear relationship between a dependent variable and one or more independent variables.

In order to optimize the model's performance and find the best fit, 
various optimization techniques can be used.

In this project, we will explore my implementation, line by line, of different optimization algorithms
and how different optimization techniques can be applied to a linear regression problem
and visualize the change of the loss and parameters' values with iterations.
Here are some common optimization algorithms that you will find in the project:

1. **Batch Gradient Descent (BGD)**: This optimizer computes the gradient of the loss function with respect to the parameters using the entire training dataset at each iteration.

2. **Stochastic Gradient Descent (SGD)**: In this optimizer, the gradient is computed based on a single randomly selected training example at each iteration. It is more computationally efficient than BGD but can have higher variance.

3. **Mini-Batch Gradient Descent (MBGD)**: MBGD is a compromise between BGD and SGD. It computes the gradient using a mini-batch of randomly selected training examples at each iteration.

4. **Momentum-based Gradient Descent**: This optimizer uses a momentum term to accelerate convergence by considering the past gradients. It helps overcome local optima and speeds up learning.

5. **Nesterov Accelerated Gradient (NAG)**: NAG is an extension of momentum-based gradient descent that calculates the gradient at a "lookahead" position, which helps improve convergence near the minimum.

6. **Adaptive Gradient Algorithm (Adagrad)**: Adagrad adapts the learning rate for each parameter based on its historical gradients. It performs larger updates for infrequent parameters and smaller updates for frequent parameters.

7. **Root Mean Squared Propagation (RMSProp)**: RMSProp addresses the diminishing learning rate problem in Adagrad by using a moving average of squared gradients. It adapts the learning rate based on the magnitudes of recent gradients.

8. **Adam**: Adam combines the benefits of momentum-based gradient descent and RMSProp. It maintains both a decaying average of past gradients and a moving average of squared gradients to adapt the learning rate.

9. **Broyden-Fletcher-Goldfarb-Shanno (BFGS)**: BFGS is a popular optimization algorithm for unconstrained problems. It approximates the inverse Hessian matrix and updates it iteratively to find the optimal solution.
