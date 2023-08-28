# Neural Network Architecture
## Combining Models
- We will combine two linear models to get our non-linear model. Essentially the steps to do this are:
   - Calculate the probability for each model
   - Apply weights to the probabilities
   - Add the weighted probabilities
   - Apply the sigmoid function to the result
## Neural networks have a certain special architecture with layers:
   - The first layer is called the input layer, which contains the inputs.
  -  The next layer is called the hidden layer, which is the set of linear models created with the input layer.
   - The final layer is called the output layer, which is where the linear models get combined to obtain a nonlinear model.

## Neural networks can have different architectures, with varying numbers of nodes and layers:
   - Input nodes. In general, if we have nn nodes in the input layer, then we are modeling data in n-dimensional space (e.g., 3 nodes in the input layer means we are modeling data in 3-dimensional space).
   - Output nodes. If there are more nodes in the output layer, this simply means we have more outputs—for example, we may have a multiclass classification model.
   - Layers. If there are more layers then we have a deep neural network. Our linear models combine to create nonlinear models, which then combine to create even more nonlinear models!

## Multi-Class Classification

- And here we elaborate a bit more into what can be done if our neural network needs to model data with more than one output.
- When we have three or more classes, we could construct three separate neural networks—one for predicting each class. However, this is not necessary. Instrad, we can add more nodes in the output layer. Each of these nodes will give us the probability that the item belongs to the given class.
