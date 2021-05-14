END-2.0-Assignments
What is a neural network neuron? Neurons in neural networks are the one that store temporary values after applying the activation function to the function containing weighted sum of input values for a given hidden layer.

What is the use of the learning rate? The objective of the Gradient Descent or any optimisation algortithm is to minimize the loss. To achieve that one can start with some initial values of weight and then move toward the global or local optima one step at a time. The learning rate is used to determine the step size by mutiplying the partial derivative of the loss function wrt that particular weight. Larger the learning rate, bigger is the step size and vice versa. The learning rate have value between 0.0 and 1.0. We need to choice the optimum value of learning rate so that the algorithm doen't skip the mimima(large learning rate) and doesn't take forever to converge(very small learning rate)

How are weights initialized? Weights can be initialised using Random Initialization but to avoid slow convergence or vanishing gradient problem, He Initializtaion and Xavier initialization can also be used.

What is "loss" in a neural network? "Loss" is the objective function that we intend to minimise. Loss function is used to adjust the weights to make bring the predictions as close to actual values as possible.

What is the "chain rule" in gradient flow? The algorithm used to update the model parameters(weights, biases) in order to effectively train a neural network is known as chain rule. Mathematically total output gradient is the total gradient caused by the all the neurons which are contributed for a output:

FinalGradient = GradientContribution1 + GradientContribution2+ ....+ GradientContributionN

Gradient(i) = GradientInside × GradientContribution(i)
