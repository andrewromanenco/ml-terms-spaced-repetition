#fundamentals

The less common label in a
[[class-imbalanced dataset|class-imbalanced dataset]]. For example,
given a dataset containing 99% negative labels and 1% positive labels, the
positive labels are the minority class.

Contrast with [[majority class|majority class]].

<section class="expandable">

<h4 class="showalways" id="click-the-icon-for-additional-notes._11" data-text=" Click the icon for additional notes. " tabindex="-1">
Click the icon for additional notes.
</h4>

<div class="expand-background">

A training set with a million <a href="#example">examples</a> sounds
impressive. However, if the minority class is poorly represented,
then even a very large training set might be insufficient. Focus less
on the total number of examples in the dataset and more on the number of
examples in the minority class.



If your dataset doesn't contain enough minority class examples, consider
using <a href="#downsampling"><b>downsampling</b></a> (the definition
in the second bullet) to supplement the minority class.

</div>

<hr />
</section>

