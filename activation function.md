#fundamentals

A function that enables [[neural network|neural networks]] to learn
[[nonlinear|nonlinear]] (complex) relationships between features
and the label.

Popular activation functions include:

<ul>
<li>[[ReLU|ReLU]]</li>
<li>[[sigmoid function|Sigmoid]]</li>
</ul>

The plots of activation functions are never single straight lines.
For example, the plot of the ReLU activation function consists of
two straight lines:


![[ images/relu.svg ]]


A plot of the sigmoid activation function looks as follows:


![[ images/sigmoid.svg ]]


<section class="expandable">

<h4 class="showalways" id="click-the-icon-to-see-an-example." data-text=" Click the icon to see an example. " tabindex="-1">
Click the icon to see an example.
</h4>

<div class="expand-background">

In a neural network, activation functions manipulate the
<a href="#weighted_sum">weighted sum</a> of all the inputs to a
<a href="#neuron">neuron</a>. To calculate a weighted sum, the neuron adds up
the products of the relevant values and weights. For example, suppose the
relevant input to a neuron consists of the following:

<table>
  <tr><td>input value</td> <td>input weight</td></tr>
  <tr><td>2</td> <td>-1.3</td></tr>
  <tr><td>-1</td> <td>0.6</td></tr>
  <tr><td>3</td> <td>0.4</td></tr>
</table>

The weighted sum is therefore:

<pre class="prettyprint" translate="no" dir="ltr">
weighted sum = (2)(-1.3) + (-1)(0.6) + (3)(0.4) = -2.0
</pre>

Suppose the designer of this neural network chooses the
<a href="#sigmoid-function"><b>sigmoid function</b></a> to be the
activation function. In that case, the neuron calculates the
sigmoid of -2.0, which is approximately 0.12. Therefore, the
neuron passes 0.12 (rather than -2.0) to the next layer in the neural network.
The following figure illustrates the relevant part of the process:


![[ images/ActivationFunction_sigmoid.png ]]

</div>

<hr />
</section>

