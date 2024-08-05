#fundamentals

In a [[binary classification|binary classification]], a
number between 0 and 1 that converts the raw output of a
[[logistic regression|logistic regression]] model
into a prediction of either the [[positive class|positive class]]
or the [[negative class|negative class]].
Note that the classification threshold is a value that a human chooses,
not a value chosen by model training.

A logistic regression model outputs a raw value between 0 and 1. Then:

<ul>
<li>If this raw value is <em>greater than</em> the classification threshold, then
the positive class is predicted.</li>
<li>If this raw value is <em>less than</em> the classification threshold, then
the negative class is predicted.</li>
</ul>

For example, suppose the classification threshold is 0.8. If the raw value
is 0.9, then the model predicts the positive class. If the raw value is
0.7, then the model predicts the negative class.

The choice of classification threshold strongly influences the number of
[[false positive (FP)|false positives]] and
[[false negative (FN)|false negatives]].

<section class="expandable">

<h4 class="showalways" id="click-the-icon-for-additional-notes._2" data-text=" Click the icon for additional notes. " tabindex="-1">
Click the icon for additional notes.
</h4>

<div class="expand-background">

As models or datasets evolve, engineers sometimes also change the
classification threshold. When the classification threshold changes,
positive class predictions can suddenly become negative classes
and vice-versa.



For example, consider a binary classification disease prediction model.
Suppose that when the system runs in the first year:

<ul>
<li>The raw value for a particular patient is 0.95.</li>
<li>The classification threshold is 0.94.</li>
</ul>

Therefore, the system diagnoses the positive class. (The patient gasps,
"Oh no! I'm sick!")

A year later, perhaps the values now look as follows:

<ul>
<li>The raw value for the same patient remains at 0.95.</li>
<li>The classification threshold changes to 0.97.</li>
</ul>

Therefore, the system now reclassifies that patient as the negative class.
("Happy day! I'm not sick.") Same patient. Different diagnosis.

</div>

<hr />
</section>

