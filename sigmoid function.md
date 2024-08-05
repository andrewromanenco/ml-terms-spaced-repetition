#fundamentals

A mathematical function that &quot;squishes&quot; an input value into a constrained range,
typically 0 to 1 or -1 to +1. That is, you can pass any number (two, a million,
negative billion, whatever) to a sigmoid and the output will still be in the
constrained range.
A plot of the sigmoid activation function looks as follows:


![[ images/sigmoid.svg ]]


The sigmoid function has several uses in machine learning, including:

<ul>
<li>Converting the raw output of a
[[logistic regression|logistic regression]]
or [[multinomial regression|multinomial regression]] model to
a probability.</li>
<li>Acting as an [[activation function|activation function]] in some
neural networks.</li>
</ul>

<section class="expandable">

<h4 class="showalways" id="click-the-icon-to-see-the-math._4" data-text=" Click the icon to see the math. " tabindex="-1">
Click the icon to see the math.
</h4>

<div class="expand-background">

The sigmoid function over an input number <i>x</i> has the following formula:


<div>
$$
sigmoid(x) = \frac{1}{1 + e^{-\text{x}}}
$$
</div>


In machine learning, <i>x</i> is generally a
<a href="#weighted_sum"><b>weighted sum</b></a>.


</div>

<hr />
</section>

