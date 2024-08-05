#fundamentals

Any mechanism that reduces [[overfitting|overfitting]].
Popular types of regularization include:

<ul>
<li><a href="#L1_regularization"><strong>L<sub>1</sub> regularization</strong></a></li>
<li><a href="#L2_regularization"><strong>L<sub>2</sub> regularization</strong></a></li>
<li>[[dropout regularization|dropout regularization]]</li>
<li>[[early stopping|early stopping]] (this is not a formal
regularization method, but can effectively limit overfitting)</li>
</ul>

Regularization can also be defined as the penalty on a model&#39;s complexity.

<section class="expandable">

<h4 class="showalways" id="click-the-icon-for-additional-notes._14" data-text=" Click the icon for additional notes. " tabindex="-1">
Click the icon for additional notes.
</h4>

<div class="expand-background">

Regularization is counterintuitive. Increasing regularization usually
<i>increases</i> training loss, which is confusing because, well, isn't
the goal to <i>minimize</i> training loss?



Actually, no. The goal isn't to minimize training loss. The goal is to
make excellent predictions on real-world examples.  Remarkably, even though
increasing regularization increases training loss, it usually helps models make
better predictions on real-world examples.


</div>

<hr />
</section>

