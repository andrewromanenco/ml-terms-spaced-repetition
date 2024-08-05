#fundamentals

A [[feature|feature]] not present among the input features, but
assembled from one or more of them. Methods for creating synthetic features
include the following:

<ul>
<li>[[bucketing|Bucketing]] a continuous feature into range bins.</li>
<li>Creating a [[feature cross|feature cross]].</li>
<li>Multiplying (or dividing) one feature value by other feature value(s)
or by itself. For example, if <code translate="no" dir="ltr">a</code> and <code translate="no" dir="ltr">b</code> are input features, then the
following are examples of synthetic features:
<ul>
  <li><tt>ab</tt></li>
  <li><tt>a<sup>2</sup></tt></li>
</ul></li>
<li>Applying a transcendental function to a feature value. For example, if <code translate="no" dir="ltr">c</code>
is an input feature, then the following are examples of synthetic features:
<ul>
  <li><tt>sin(c)</tt></li>
  <li><tt>ln(c)</tt></li>
</ul></li>
</ul>

Features created by [[normalization|normalizing]] or [[scaling|scaling]]
alone are not considered synthetic features.


