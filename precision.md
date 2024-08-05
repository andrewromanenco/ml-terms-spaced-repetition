
A metric for [[classification model|classification models]] that answers
the following question:

<blockquote>
When the model predicted the [[positive class|positive class]],
what percentage of the predictions were correct?
</blockquote>

Here is the formula:

<div>
$$\text{Precision} =
\frac{\text{true positives}} {\text{true positives} + \text{false positives}}$$
</div>

where:

<ul>
<li>true positive means the model <em>correctly</em> predicted the positive class.</li>
<li>false positive means the model <em>mistakenly</em> predicted the positive class.</li>
</ul>

For example, suppose a model made 200 positive predictions.
Of these 200 positive predictions:

<ul>
<li>150 were true positives.</li>
<li>50 were false positives.</li>
</ul>

In this case:

<div>
$$\text{Precision} =
\frac{\text{150}} {\text{150} + \text{50}} = 0.75$$
</div>

Contrast with [[accuracy|accuracy]] and [[recall|recall]].

