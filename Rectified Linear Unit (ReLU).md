#fundamentals

An [[activation function|activation function]] with the following behavior:

<ul>
<li>If input is negative or zero, then the output is 0.</li>
<li>If input is positive, then the output is equal to the input.</li>
</ul>

For example:

<ul>
<li>If the input is -3, then the output is 0.</li>
<li>If the input is +3, then the output is 3.0.</li>
</ul>

Here is a plot of ReLU:


![[ images/ReLU.png ]]


ReLU is a very popular activation function. Despite its simple behavior,
ReLU still enables a neural network to learn [[nonlinear|nonlinear]]
relationships between [[feature|features]] and the [[label|label]].

