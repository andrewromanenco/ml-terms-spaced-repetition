
A metric for [[classification model|classification models]] that answers
the following question:

<blockquote>
When [[ground truth|ground truth]] was the
[[positive class|positive class]], what percentage of predictions did
the model correctly identify as the positive class?
</blockquote>

Here is the formula:

\[\text{Recall} =
\frac{\text{true positives}} {\text{true positives} + \text{false negatives}}
\]

where:

<ul>
<li>true positive means the model <em>correctly</em> predicted the positive class.</li>
<li>false negative means that the model <em>mistakenly</em> predicted the
[[negative class|negative class]].</li>
</ul>

For instance, suppose your model made 200 predictions on examples for which
ground truth was the positive class. Of these 200 predictions:

<ul>
<li>180 were true positives.</li>
<li>20 were false negatives.</li>
</ul>

In this case:

\[\text{Recall} =
\frac{\text{180}} {\text{180} + \text{20}} = 0.9
\]

<section class="expandable">

<h4 class="showalways" id="click-the-icon-for-notes-about-class-imbalanced-datasets." data-text=" Click the icon for notes about class-imbalanced datasets. " tabindex="-1">
Click the icon for notes about class-imbalanced datasets.
</h4>

<div class="expand-background">

Recall is particularly useful for determining the predictive power of
classification models in which the positive class is rare. For example, consider
a <a href="#class_imbalanced_data_set"><b>class-imbalanced dataset</b></a>
in which the positive class for a certain disease occurs in only 10 patients
out of a million. Suppose your model makes five million predictions that yield
the following outcomes:


<ul>
  <li>30 True Positives</li>
  <li>20 False Negatives</li>
  <li>4,999,000 True Negatives</li>
  <li>950 False Positives</li>
</ul>

The recall of this model is therefore:

<pre translate="no" dir="ltr">
recall = TP / (TP + FN)
recall = 30 / (30 + 20) = 0.6 = 60%
</pre>

By contrast, the <a href="#accuracy">accuracy</a> of this model is:

<pre translate="no" dir="ltr">
accuracy = (TP + TN) / (TP + TN + FP + FN)
accuracy = (30 + 4,999,000) / (30 + 4,999,000 + 950 + 20) = 99.98%
</pre>


That high value of accuracy looks impressive but is essentially meaningless.
Recall is a much more useful metric for class-imbalanced datasets than accuracy.

</div>

<hr />
</section>

