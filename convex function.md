
A function in which the region above the graph of the function is a
[[convex set|convex set]]. The prototypical convex function is
shaped something like the letter <strong>U</strong>. For example, the following
are all convex functions:


![[ images/convex_functions.png ]]


In contrast, the following function is not convex. Notice how the
region above the graph is not a convex set:


![[ images/nonconvex_function.svg ]]


A <strong>strictly convex function</strong> has exactly one local minimum point, which
is also the global minimum point. The classic U-shaped functions are
strictly convex functions. However, some convex functions
(for example, straight lines) are not U-shaped.

<section class="expandable">

<h4 class="showalways" id="click-the-icon-for-a-deeper-look-at-the-math." data-text=" Click the icon for a deeper look at the math. " tabindex="-1">
Click the icon for a deeper look at the math.
</h4>

<div class="expand-background">

A lot of the common <a href="#loss-function">loss functions</a>, including the
following, are convex functions:


<ul>
<li><a href="#L2_loss"><b>L<sub>2</sub> loss</b></a></li>
<li><a href="#Log_Loss"><b>Log Loss</b></a></li>
<li><a href="#L1_regularization"><b>L<sub>1</sub> regularization</b></a></li>
<li><a href="#L2_regularization"><b>L<sub>2</sub> regularization</b></a></li>
</ul>


Many variations of <a href="#gradient_descent"><b>gradient descent</b></a>
are guaranteed to find a point close to the minimum of a
strictly convex function. Similarly, many variations of
<a href="#SGD"><b>stochastic gradient descent</b></a> have a high probability
(though, not a guarantee) of finding a point close to the minimum of a
strictly convex function.



The sum of two convex functions (for example,
L<sub>2</sub> loss + L<sub>1</sub> regularization) is a convex function.



<a href="#deep_model"><b>Deep models</b></a> are never convex functions.
Remarkably, algorithms designed for
<a href="#convex_optimization"><b>convex optimization</b></a> tend to find
reasonably good solutions on deep networks anyway, even though
those solutions are not guaranteed to be a global minimum.

</div>

<hr />
</section>

