#fundamentals

A floating-point number that tells the [[gradient descent|gradient descent]]
algorithm how strongly to adjust weights and biases on each
[[iteration|iteration]]. For example, a learning rate of 0.3 would
adjust weights and biases three times more powerfully than a learning rate
of 0.1.

Learning rate is a key [[hyperparameter|hyperparameter]]. If you set
the learning rate too low, training will take too long. If
you set the learning rate too high, gradient descent often has trouble
reaching [[convergence|convergence]].

<section class="expandable">

<h4 class="showalways" id="click-the-icon-for-a-more-mathematical-explanation." data-text=" Click the icon for a more mathematical explanation. " tabindex="-1">
Click the icon for a more mathematical explanation.
</h4>

<div class="expand-background">

During each iteration, the
<a href="#gradient_descent"><b>gradient descent</b></a>
algorithm multiplies the
learning rate by the gradient. The resulting product is called the
<b>gradient step</b>.

</div>

<hr />
</section>

