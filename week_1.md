### Week 1


#### Supervised v Unsupervised

* Machine Learning: computers the ability to learn without being explicitly programmed
* Supervised Learning: learns with output label 

#### Gradient descent

This method can be used on any cost function, not just linear regression 


1. Objective: minimise the cost function
2. Start with initial values: w,b
3. Keep changin w,b to reduce the cost function
4. Continue till reach a local minimum 

##### Gradient descent algorithm:

Simultaneously update w and b
$$w = w - \alpha \frac{\partial }{\partial w} J(w,b) $$
$$b = b - \alpha \frac{\partial }{\partial b} J(w,b)$$

Learning rate is the alpha parameter, if alpha is too small there will be many iterations of adjusting paramters and cost function. Meaning it will eventually find local minimum but will take longer. If alpha is too big, we can jump over local minimums and may not be able to find local minimum. 

The squared error cost function with linear regression, the cost function does not and will never have multiple local minima, it has one global minima as it is a convex function. 
