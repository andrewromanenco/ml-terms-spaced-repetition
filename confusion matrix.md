#fundamentals

An NxN table that summarizes the number of correct and incorrect predictions
that a [[classification model|classification model]] made.
For example, consider the following confusion matrix for a
[[binary classification|binary classification]] model:

<table>
<thead>
<tr>
<th></th>
<th>Tumor (predicted)</th>
<th>Non-Tumor (predicted)</th>
</tr>
</thead>

<tbody>
<tr>
<td>Tumor (ground truth)</td>
<td>18 (TP)</td>
<td>1 (FN)</td>
</tr>
<tr>
<td>Non-Tumor (ground truth)</td>
<td>6 (FP)</td>
<td>452 (TN)</td>
</tr>
</tbody>
</table>

The preceding confusion matrix shows the following:

<ul>
<li>Of the 19 predictions in which [[ground truth|ground truth]] was Tumor,
the model correctly classified 18 and incorrectly classified 1.</li>
<li>Of the 458 predictions in which ground truth was Non-Tumor, the model
correctly classified 452 and incorrectly classified 6.</li>
</ul>

The confusion matrix for a [[multi-class classification|multi-class classification]]
problem can help you identify patterns of mistakes.
For example, consider the following confusion matrix for a 3-class
multi-class classification model that categorizes three different iris types
(Virginica, Versicolor, and Setosa). When the ground truth was Virginica, the
confusion matrix shows that the model was far more likely to mistakenly
predict Versicolor than Setosa:

<table>
  <tr>
    <th>&nbsp;</th>
    <th>Setosa (predicted)</th>
    <th>Versicolor (predicted)</th>
    <th>Virginica (predicted)</th>
  </tr>
  <tr>
    <td>Setosa (ground truth)</td>
    <td>88</td>
    <td>12</td>
    <td>0</td>
  </tr>
  <tr>
    <td>Versicolor (ground truth)</td>
    <td>6</td>
    <td>141</td>
    <td>7</td>
  </tr>
  <tr>
    <td>Virginica (ground truth)</td>
    <td>2</td>
    <td>27</td>
    <td>109</td>
  </tr>
</table>

As yet another example, a confusion matrix could reveal that a model trained
to recognize handwritten digits tends to mistakenly predict 9 instead of 4,
or mistakenly predict 1 instead of 7.

Confusion matrixes contain sufficient information to calculate a
variety of performance metrics, including [[precision|precision]]
and [[recall|recall]].

