#fundamentals

A number that specifies the relative importance of
[[regularization|regularization]] during training. Raising the
regularization rate reduces [[overfitting|overfitting]] but may
reduce the model&#39;s predictive power. Conversely, reducing or omitting
the regularization rate increases overfitting.

<section class="expandable">

<h4 class="showalways" id="click-the-icon-to-see-the-math._3" data-text=" Click the icon to see the math. " tabindex="-1">
Click the icon to see the math.
</h4>

<div class="expand-background">

The regularization rate is usually represented as the Greek letter lambda.
The following simplified <a href="#loss"><b>loss</b></a> equation shows
lambda's influence:


<div>
$$\text{minimize(loss function + }\lambda\text{(regularization))}$$
</div>

where <i>regularization</i> is any regularization mechanism, including;

<ul>
 <li><a href="#L1_regularization"><b>L<sub>1</sub> regularization</b></a></li>
 <li><a href="#L2_regularization"><b>L<sub>2</sub> regularization</b></a></li>
</ul>

</div>

<hr />
</section>

