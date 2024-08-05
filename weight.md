#fundamentals

A value that a model multiplies by another value.
[[training|Training]] is the process of determining a model&#39;s ideal weights;
[[inference|inference]] is the process of using those learned weights to
make predictions.

<section class="expandable">

<h4 class="showalways" id="click-the-icon-to-see-an-example-of-weights-in-a-linear-model." data-text=" Click the icon to see an example of weights in a linear model. " tabindex="-1">
Click the icon to see an example of weights in a linear model.
</h4>

<div class="expand-background">

Imagine a <a href="#linear_model"><b>linear model</b></a> with two features.
Suppose that training determines the following weights (and
<a href="#bias">bias</a>):


<ul>
  <li>The bias, b, has a value of 2.2</li>
  <li>The weight, w<sub>1</sub> associated with one feature is 1.5.</li>
  <li>The weight, w<sub>2</sub> associated with the other feature is 0.4.</li>
</ul>

Now imagine an <a href="#example">example</a> with the following feature
values:

<ul>
  <li>The value of one feature, x<sub>1</sub>, is 6.</li>
  <li>The value of the other feature, x<sub>2</sub>, is 10.</li>
</ul>

This linear model uses the following formula to generate a prediction,
y':

<div>
$$y' = b + w_1x_1 + w_2x_2$$
</div>

Therefore, the prediction is:

<div>
$$y' = 2.2 + (1.5)(6) + (0.4)(10) = 15.2$$
</div>

If a weight is 0, then the corresponding feature doesn't contribute to
the model. For example, if w<sub>1</sub> is 0, then the value of x<sub>1</sub>
is irrelevant.

</div>
<hr />
</section>

