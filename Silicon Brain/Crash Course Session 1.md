ETA: 1 hour

### 10 minutes: explain basic linear algebra
**What are [[Vectors|vectors]]?**

From a physics point of a view, a vector is a mathematical object with a direction and a magnitude.

From a computer science point of view, a vector is simply an array of numbers. Imagine you're buying a house, what would you care about? You'd care about the location of the house (represented in latitude and longitude), the size of the house, the price of the house, interest, etc. All of this can be represented by an array of numbers, and you can plot this array of numbers as if they were coordinates in some space.

**What are [[Matrices|matrices]]?**

Matrices are 2D arrays of numbers. You can think of them as a vector of vectors.

Matrices represent linear transforms because they represent base vectors.

#### 5 minutes: explain calculus
**What is a derivative?**

Derivative is the rate of change of a function with respect to a variable.

### 20 minutes: explain how neural networks work
Use basic feed forward neural network as a teaching tool.

**What is a neuron in an FNN?**
A neuron is simply a weight and a bias.
A neuron's weights can be thought of as a row vector.

**What is a layer?**
A layer is a group of neurons.
A layer can be thought of as a matrix.

##### What is a loss function?
A loss function is a function that takes in desired output and actual output, and outputs how wrong the actual output is from the desired output.

**Explain backpropagation.**
Backpropagation is an algorithm that calculates the gradients of each layer and each neuron, using derivatives.

**Explain gradient descent.**
Gradient descent is an algorithm that uses these gradients to modify the weights such that they are closer to an optimum.

```py
network = Network()
input = ...
desired_output = ...
epochs = 100
learning_rate = 0.01

for epoch in range(epochs):
	actual_output = network(input)
	loss = loss_function(actual_output, desired_output)
	gradients = backprop(loss, model, loss_function)
	model.weights -= learning_rate * gradients
```

### 30 minutes: explain the various architectures
explain RNN