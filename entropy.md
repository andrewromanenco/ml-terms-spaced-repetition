#df

In
<a href="https://wikipedia.org/wiki/Information_theory" target="T">
information theory</a>,
a description of how unpredictable a probability
distribution is. Alternatively, entropy is also defined as how much
information each [[example|example]] contains. A distribution has
the highest possible entropy when all values of a random variable are
equally likely.

The entropy of a set with two possible values &quot;0&quot; and &quot;1&quot; (for example,
the labels in a [[binary classification|binary classification]] problem)
has the following formula:

<tt>
&nbsp;&nbsp;H = -p log p - q log q = -p log p - (1-p) * log (1-p)
</tt>

where:

<ul>
<li><tt>H</tt> is the entropy.</li>
<li><tt>p</tt> is the fraction of &quot;1&quot; examples.</li>
<li><tt>q</tt> is the fraction of &quot;0&quot; examples. Note that q = (1 - p)</li>
<li><tt>log</tt> is generally log<sub>2</sub>. In this case, the entropy
unit is a bit.</li>
</ul>

For example, suppose the following:

<ul>
<li>100 examples contain the value &quot;1&quot;</li>
<li>300 examples contain the value &quot;0&quot;</li>
</ul>

Therefore, the entropy value is:

<ul>
  <li><tt>p = 0.25</tt></li>
  <li><tt>q = 0.75</tt></li>
  <li><tt>H = (-0.25)log<sub>2</sub>(0.25) - (0.75)log<sub>2</sub>(0.75) =
      0.81 bits per example</tt></li>
</ul>

A set that is perfectly balanced (for example, 200 &quot;0&quot;s and 200 &quot;1&quot;s)
would have an entropy of 1.0 bit per example. As a set becomes more
[[class-imbalanced dataset|imbalanced]], its entropy moves towards 0.0.

In [[decision tree|decision trees]], entropy helps formulate
[[information gain|information gain]] to help the
[[splitter|splitter]] select the [[condition|conditions]]
during the growth of a classification decision tree.

Compare entropy with:

<ul>
<li>[[gini impurity|gini impurity]]</li>
<li>[[cross-entropy|cross-entropy]] loss function</li>
</ul>

Entropy is often called Shannon&#39;s entropy.

