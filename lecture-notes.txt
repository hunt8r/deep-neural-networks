Deep Neural networks

* You will initialize the weights matrices with random values.
    * Use: np.random.randn(a,b) * 0.01 to randomly initialize a matrix of shape (a,b).
* You will initialize the bias vectors as zeros.
    * Use: np.zeros((a,b)) to initialize a matrix of shape (a,b) with zeros.

Notice the difference in initializing a np array with zeros and randn. The syntax for zeros includes additional braces.

Hyperparameters:

High variance - Higher Dev set error > Training set error
Training set error : 1%
Dev set error.       : 11%

High bias - Higher Dev set error and Higher Training set error
Training set error : 15%
Dev set error.       : 16%

High variance and bias - Much Much Higher Dev set error and Higher Training set error
Training set error : 15%
Dev set error.       : 30%

Low variance and bias - Lower Dev set error and Lower Training set error
Training set error : 0.5%
Dev set error.       : 1%

High bias?
(Training data performance)
Improved by:
    - Bigger network
    - Training longer
    - Neural Network Architectures

High variance?
(Dev set performance)
Improved by:
    - More data
    - Regularization
    - Drop 
    - Neural Network Architectures

Vanishing/exploding gradients
(Increases time to train Neural Network)
	Improved by:
	- Carefully selecting the weights using within each layer W^[L]
		- For each W, in a layer, you generate randn values within the weights and multiply by sqrt(1/n^[L-1]) or you can use tanh * sqrt(..)

Backprop check if derivatives are working fine
(Gradient checking)
	Improved by:
	- Taking 2 sided difference, you can numerically verify whether derivative is correct





