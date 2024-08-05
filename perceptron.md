
A system (either hardware or software) that takes in one or more input values,
runs a function on the weighted sum of the inputs, and computes a single
output value. In machine learning, the function is typically nonlinear, such as
[[ReLU|ReLU]], [[sigmoid function|sigmoid]], or
<a href="https://wikipedia.org/wiki/Hyperbolic_functions" target="T">tanh</a>.
For example, the following perceptron relies on the sigmoid function to process
three input values:

<div>
$$f(x_1, x_2, x_3) = \text{sigmoid}(w_1 x_1 + w_2 x_2 + w_3 x_3)$$
</div>

In the following illustration, the perceptron takes three inputs, each of which
is itself modified by a weight before entering the perceptron:


![[ images/Perceptron.svg ]]


Perceptrons are the [[neuron|neurons]] in
[[neural network|neural networks]].

