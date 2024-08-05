
The average loss per example when <a href="#L1_loss"><strong>L<sub>1</sub> loss</strong></a> is
used. Calculate Mean Absolute Error as follows:

<ol>
<li>Calculate the L<sub>1</sub> loss for a batch.</li>
<li>Divide the L<sub>1</sub> loss by the number of examples in the batch.</li>
</ol>

<section class="expandable">

<h4 class="showalways" id="click-the-icon-to-see-the-formal-math._2" data-text=" Click the icon to see the formal math. " tabindex="-1">
Click the icon to see the formal math.
</h4>

<div class="expand-background">


$$\text{Mean Absolute Error} = \frac{1}{n}\sum_{i=0}^n | y_i - \hat{y}_i |$$


where:

<ul>
  <li>$n$ is the number of examples.</li>
  <li>$y$ is the actual value of the label.</li>
  <li>$\hat{y}$ is the value that the model predicts for $y$.</li>
</ul>

</div>

<hr />
</section>

For example, consider the calculation of L<sub>1</sub> loss on the
following batch of five examples:

<table>
  <tr><th>Actual value of example</th> <th>Model's predicted value</th>
      <th>Loss (difference between actual and predicted)</th></tr>
  <tr><td>7</td> <td>6</td> <td>1</td> </tr>
  <tr><td>5</td> <td>4</td> <td>1</td> </tr>
  <tr><td>8</td> <td>11</td> <td>3</td> </tr>
  <tr><td>4</td> <td>6</td> <td>2</td> </tr>
  <tr><td>9</td> <td>8</td> <td>1</td> </tr>
  <tr><th colspan="2">&nbsp;</th>  <th>8 = L<sub>1</sub> loss</th> </tr>
</table>

So, L<sub>1</sub> loss is 8 and the number of examples is 5.
Therefore, the Mean Absolute Error is:

<pre translate="no" dir="ltr">
Mean Absolute Error = L<sub>1</sub> loss / Number of Examples
Mean Absolute Error = 8/5 = 1.6
</pre>

Contrast Mean Absolute Error with [[Mean Squared Error (MSE)|Mean Squared Error]] and
[[Root Mean Squared Error (RMSE)|Root Mean Squared Error]].

