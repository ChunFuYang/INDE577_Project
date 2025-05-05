# Neural Networks

Neural Networks are computational models inspired by the human brain, capable of learning complex patterns from data. The most common type is the feedforward neural network, also known as a multilayer perceptron (MLP).

## Structure
- **Input Layer:** Receives input features.
- **Hidden Layers:** One or more layers where computations are performed.
- **Output Layer:** Produces the final prediction.

Each neuron computes a weighted sum of its inputs, applies an activation function (e.g., sigmoid, ReLU), and passes the result to the next layer.

## Mathematical Formulation
For a single neuron:

$$
a = f\left(\sum_{i=1}^n w_i x_i + b\right)
$$

- $a$: Output of the neuron
- $f$: Activation function
- $w_i$: Weights
- $x_i$: Inputs
- $b$: Bias

## Learning
Neural networks learn by adjusting weights to minimize a loss function (e.g., cross-entropy for classification) using algorithms like backpropagation and gradient descent.

## Applications
- Image and speech recognition
- Natural language processing
- Regression and classification tasks

Neural networks can approximate complex, non-linear functions and are the foundation of deep learning.
