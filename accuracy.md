#fundamentals

The number of correct classification [[prediction|predictions]] divided
by the total number of predictions. That is:

<div>
$$\text{Accuracy} =
\frac{\text{correct predictions}} {\text{correct predictions + incorrect predictions }}$$
</div>

For example, a model that made 40 correct predictions and 10 incorrect
predictions would have an accuracy of:

<div>
$$\text{Accuracy} =
\frac{\text{40}} {\text{40 + 10}} =
\text{80%}$$
</div>

[[binary classification|Binary classification]] provides specific names
for the different categories of <em>correct predictions</em> and
<em>incorrect predictions</em>. So, the accuracy formula for binary classification
is as follows:

<div>
$$\text{Accuracy} = \frac{\text{TP} + \text{TN}}
                         {\text{TP} + \text{TN} + \text{FP} + \text{FN}}$$
</div>

where:

<ul>
<li>TP is the number of [[true positive (TP)|true positives]] (correct predictions).</li>
<li>TN is the number of [[true negative (TN)|true negatives]] (correct predictions).</li>
<li>FP is the number of [[false positive (FP)|false positives]] (incorrect predictions).</li>
<li>FN is the number of [[false negative (FN)|false negatives]] (incorrect predictions).</li>
</ul>

Compare and contrast accuracy with
[[precision|precision]] and
[[recall|recall]].

<section class="expandable">

<h4 class="showalways" id="click-the-icon-for-additional-notes." data-text=" Click the icon for additional notes. " tabindex="-1">
Click the icon for additional notes.
</h4>

<div class="expand-background">

Although a valuable metric for some situations, accuracy is highly
misleading for others. Notably, accuracy is usually a poor metric
for evaluating classification models that process
<a href="#class_imbalanced_data_set"><b>class-imbalanced datasets</b></a>.



For example, suppose snow falls only 25 days per century in a certain
subtropical city. Since days without snow (the negative class) vastly
outnumber days with snow (the positive class), the snow dataset for
this city is class-imbalanced.
Imagine a <a href="#binary-classification"><b>binary classification</b></a>
model that is supposed to predict either snow or no snow each day but
simply predicts "no snow" every day.
This model is highly accurate but has no predictive power.
The following table summarizes the results for a century of predictions:


<table>
  <tr><th>Category</th> <th>Number</th> </tr>
  <tr><td>TP</td> <td>0</td>     </tr>
  <tr><td>TN</td> <td>36500</td> </tr>
  <tr><td>FP</td> <td>25</td>    </tr>
  <tr><td>FN</td> <td>0</td>     </tr>
</table>

The accuracy of this model is therefore:

<pre class="prettyprint" translate="no" dir="ltr">
accuracy = (TP + TN) / (TP + TN + FP + FN)
accuracy = (0 + 36500) / (0 + 36500 + 25 + 0) = 0.9993 = 99.93%
</pre>

Although 99.93% accuracy seems like very a impressive percentage, the model
actually has no predictive power.


<a href="#precision"><b>Precision</b></a> and
<a href="#recall"><b>recall</b></a> are usually more useful metrics
than <b>accuracy</b> for evaluating models trained on class-imbalanced datasets.

</div>

<hr />
</section>

