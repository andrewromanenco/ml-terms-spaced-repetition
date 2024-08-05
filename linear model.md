#fundamentals

A [[model|model]] that assigns one [[weight|weight]] per
[[feature|feature]] to make [[prediction|predictions]].
(Linear models also incorporate a [[bias (math) or bias term|bias]].) In contrast,
the relationship of features to predictions in [[deep model|deep models]]
is generally <strong>nonlinear</strong>.

Linear models are usually easier to train and more
[[interpretability|interpretable]] than deep models. However,
deep models can learn complex relationships <em>between</em> features.

[[linear regression|Linear regression]] and
[[logistic regression|logistic regression]] are two types of linear models.

<section class="expandable">

<h4 class="showalways" id="click-the-icon-to-see-the-math." data-text=" Click the icon to see the math. " tabindex="-1">
Click the icon to see the math.
</h4>

<div class="expand-background">
A linear model follows this formula:

<div>
$$y' = b + w_1x_1 + w_2x_2 + … w_nx_n$$
</div>

where:
<ul>
<li>y' is the raw prediction. (In certain kinds of linear models, this
raw prediction will be further modified. For example, see
<a href="#logistic_regression"><b>logistic regression</b></a>.)</li>
<li>b is the <a href="#bias"><b>bias</b></a>.</li>
<li>w is a <a href="#weight"><b>weight</b></a>, so w<sub>1</sub> is
the weight of the first feature, w<sub>2</sub> is the weight of the
second feature, and so on.</li>
<li>x is a <a href="#feature"><b>feature</b></a>, so x<sub>1</sub> is the
value of the first feature, x<sub>2</sub> is the value of the second feature,
and so on.</li>
</ul>

For example, suppose a linear model for three features learns the following
bias and weights:
<ul>
<li>b = 7</li>
<li>w<sub>1</sub> = -2.5</li>
<li>w<sub>2</sub> = -1.2</li>
<li>w<sub>3</sub> = 1.4</li>
</ul>

Therefore, given three features (x<sub>1</sub>, x<sub>2</sub>,
and x<sub>3</sub>), the linear model uses the following equation
to generate each prediction:

<pre translate="no" dir="ltr">
y' = 7 + (-2.5)(x<sub>1</sub>) + (-1.2)(x<sub>2</sub>) + (1.4)(x<sub>3</sub>)
</pre>

Suppose a particular example contains the following values:

<ul>
<li>x<sub>1</sub> = 4</li>
<li>x<sub>2</sub> = -10</li>
<li>x<sub>3</sub> = 5</li>
</ul>

Plugging those values into the formula yields a prediction for this example:

<pre translate="no" dir="ltr">
y' = 7 + (-2.5)(4) + (-1.2)(-10) + (1.4)(5)
y' = 16
</pre>

Linear models include not only models that use only a linear equation to
make predictions but also a broader set of models that use a linear equation
as just one component of the formula that makes predictions.
For example, logistic regression post-processes the raw
prediction (y') to produce a final prediction value between 0 and 1,
exclusively.

</div>

<hr />
</section>

