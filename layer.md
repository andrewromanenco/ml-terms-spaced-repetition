#fundamentals

A set of [[neuron|neurons]] in a
[[neural network|neural network]]. Three common types of layers
are as follows:

<ul>
<li>The [[input layer|input layer]], which provides values for all the
[[feature|features]].</li>
<li>One or more [[hidden layer|hidden layers]], which find
nonlinear relationships between the features and the label.</li>
<li>The [[output layer|output layer]], which provides the prediction.</li>
</ul>

For example, the following illustration shows a neural network with
one input layer, two hidden layers, and one output layer:


![[ images/Layers.png ]]


In [[TensorFlow|TensorFlow]], <strong>layers</strong> are also Python functions that take
[[Tensor|Tensors]] and configuration options as input and
produce other tensors as output.

