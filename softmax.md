#fundamentals

A function that determines probabilities for each possible class in a
[[multi-class classification|multi-class classification model]]. The probabilities add up
to exactly 1.0. For example, the following table shows how softmax distributes
various probabilities:

<table>
  <tr><th>Image is a...</th> <th>Probability</th></tr>
  <tr><td>dog</td>           <td>.85</td></tr>
  <tr><td>cat</td>           <td>.13</td></tr>
  <tr><td>horse</td>         <td>.02</td></tr>
</table>

Softmax is also called <strong>full softmax</strong>.

Contrast with [[candidate sampling|candidate sampling]].

<section class="expandable">

<h4 class="showalways" id="click-the-icon-to-see-the-math._5" data-text=" Click the icon to see the math. " tabindex="-1">
Click the icon to see the math.
</h4>

<div class="expand-background">
The softmax equation is as follows:

<div>
$$\sigma_i = \frac{e^{\text{z}_i}} {\sum_{j=1}^{j=K} {e^{\text{z}_j}}} $$
</div>

where:

<ul>
<li>$\sigma_i$ is the output vector. Each element of the output vector
specifies the probability of this element. The sum of all the elements
in the output vector is 1.0. The output vector contains the same number
of elements as the input vector, $z$.</li>
<li>$z$ is the input vector. Each element of the input vector contains
a floating-point value.</li>
<li>$K$ is the number of elements in the input vector (and the output
vector).</li>
</ul>

For example, suppose the input vector is:

<pre translate="no" dir="ltr">
[1.2, 2.5, 1.8]
</pre>

Therefore, softmax calculates the denominator as follows:

<div>
$$\text{denominator} = e^{1.2} + e^{2.5} + e^{1.8} = 21.552$$
</div>

The softmax probability of each element is therefore:

<div>
$$\sigma_1 = \frac{e^{1.2}}{21.552} = 0.154 $$
$$\sigma_2 = \frac{e^{2.5}}{21.552} = 0.565 $$
$$\sigma_1 = \frac{e^{1.8}}{21.552} = 0.281 $$
</div>

So, the output vector is therefore:

<div>
$$\sigma = [0.154, 0.565, 0.281]$$
</div>

The sum of the three elements in $\sigma$ is 1.0. Phew!

</div>

<hr />
</section>

