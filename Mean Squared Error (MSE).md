
The average loss per example when <a href="#L2_loss"><strong>L<sub>2</sub> loss</strong></a> is
used. Calculate Mean Squared Error as follows:

<ol>
<li>Calculate the L<sub>2</sub> loss for a batch.</li>
<li>Divide the L<sub>2</sub> loss by the number of examples in the batch.</li>
</ol>

<section class="expandable">

<h4 class="showalways" id="click-the-icon-to-see-the-formal-math._3" data-text=" Click the icon to see the formal math. " tabindex="-1">
Click the icon to see the formal math.
</h4>

<div class="expand-background">

$$\text{Mean Squared Error} = \frac{1}{n}\sum_{i=0}^n {(y_i - \hat{y}_i)}^2$$

where:

<ul>
  <li>$n$ is the number of examples.</li>
  <li>$y$ is the actual value of the label.</li>
  <li>$\hat{y}$ is the model's prediction for $y$.</li>
</ul>
</div>

<hr />
</section>

For example, consider the loss on the following batch of five examples:

<table>
  <tr><th>Actual value</th> <th>Model's prediction</th>
      <th>Loss</th> <th>Squared loss</th></tr>
  <tr><td>7</td> <td>6</td>  <td>1</td> <td>1</td></tr>
  <tr><td>5</td> <td>4</td>  <td>1</td> <td>1</td></tr>
  <tr><td>8</td> <td>11</td> <td>3</td> <td>9</td></tr>
  <tr><td>4</td> <td>6</td>  <td>2</td> <td>4</td></tr>
  <tr><td>9</td> <td>8</td>  <td>1</td> <td>1</td></tr>
  <tr><th colspan="3"> </th> <th>16 = L<sub>2</sub> loss</th></tr>
</table>

Therefore, the Mean Squared Error is:

<pre translate="no" dir="ltr">
Mean Squared Error = L<sub>2</sub> loss / Number of Examples
Mean Squared Error = 16/5 = 3.2
</pre>

Mean Squared Error is a popular training [[optimizer|optimizer]],
particularly for [[linear regression|linear regression]].

Contrast Mean Squared Error with
[[Mean Absolute Error (MAE)|Mean Absolute Error]] and
[[Root Mean Squared Error (RMSE)|Root Mean Squared Error]].

[[TensorFlow Playground|TensorFlow Playground]] uses Mean Squared Error
to calculate loss values.

<section class="expandable">

<h4 class="showalways" id="click-the-icon-to-see-more-details-about-outliers." data-text=" Click the icon to see more details about outliers. " tabindex="-1">
Click the icon to see more details about outliers.
</h4>

<div class="expand-background">


<a href="#outliers"><b>Outliers</b></a> strongly influence Mean Squared Error.
For example, a loss of 1 is a squared loss of 1, but a loss of 3 is a
squared loss of 9. In the preceding table, the example with a loss of 3
accounts for ~56% of the Mean Squared Error, while each of the examples
with a loss of 1 accounts for only 6% of the Mean Squared Error.


Outliers don't influence Mean Absolute Error as strongly as
Mean Squared Error. For example, a loss of 3 accounts for only ~38% of the
Mean Absolute Error.

<a href="#clipping"><b>Clipping</b></a> is one way to prevent extreme
outliers from damaging your model's predictive ability.

</div>

<hr />
</section>

