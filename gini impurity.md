#df

A metric similar to [[entropy|entropy]]. [[splitter|Splitters]]
use values derived from either gini impurity or entropy to compose
[[condition|conditions]] for classification
[[decision tree|decision trees]].
[[information gain|Information gain]] is derived from entropy.
There is no universally accepted equivalent term for the metric derived
from gini impurity; however, this unnamed metric is just as important as
information gain.

Gini impurity is also called <strong>gini index</strong>, or simply <strong>gini</strong>.

<section class="expandable">

<h4 class="showalways" id="click-the-icon-for-mathematical-details-about-gini-impurity." data-text=" Click the icon for mathematical details about gini impurity. " tabindex="-1">
Click the icon for mathematical details about gini impurity.
</h4>

<div class="expand-background">
Gini impurity is the probability of misclassifying a new piece of data
taken from the same distribution. The gini impurity of a set with two
possible values "0" and "1" (for example, the labels in a
<b><a href="#binary_classification">binary classification</a></b> problem)
is calculated from the following formula:


<tt>&nbsp;&nbsp;
I = 1 - (p<sup>2</sup> + q<sup>2</sup>) = 1 - (p<sup>2</sup> + (1-p)<sup>2</sup>)
</tt>


where:

<ul>
  <li><tt>I</tt> is the gini impurity.</li>
  <li><tt>p</tt> is the fraction of "1" examples.</li>
  <li><tt>q</tt> is the fraction of "0" examples. Note that <tt>q =
  1-p</tt></li>
</ul>

For example, consider the following dataset:

<ul>
  <li>100 labels (0.25 of the dataset) contain the value "1"</li>
  <li>300 labels (0.75 of the dataset) contain the value "0"</li>
</ul>

Therefore, the gini impurity is:

<ul>
  <li><tt>p = 0.25</tt></li>
  <li><tt>q = 0.75</tt></li>
  <li><tt>I = 1 - (0.25<sup>2</sup> + 0.75<sup>2</sup>) = <b>0.375</b></tt></li>
</ul>

Consequently, a random label from the same dataset would have a 37.5% chance
of being misclassified, and a 62.5% chance of being properly classified.

A perfectly balanced label (for example, 200 "0"s and 200 "1"s) would have a
gini impurity of 0.5. A highly
<a href="#class_imbalanced_data_set"><b>imbalanced</b></a> label would have a
gini impurity close to 0.0.
</div>

<hr />
</section>

