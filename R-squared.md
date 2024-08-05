
A [[regression model|regression]] metric indicating how much variation in a
[[label|label]] is due to an individual feature or to a feature set.
R-squared is a value between 0 and 1, which you can interpret as follows:

<ul>
<li>An R-squared of 0 means that none of a label&#39;s variation is due to the
feature set.</li>
<li>An R-squared of 1 means that all of a label&#39;s variation is due to the
feature set.</li>
<li>An R-squared between 0 and 1 indicates the extent to which the label&#39;s
variation can be predicted from a particular feature or the feature set.
For example, an R-squared of 0.10 means that 10 percent of the variance
in the label is due to the feature set, an R-squared of 0.20 means that
20 percent is due to the feature set, and so on.</li>
</ul>

R-squared is the square of the
<a href="https://wikipedia.org/wiki/Correlation_coefficient">Pearson correlation
coefficient</a>
between the values that a model predicted and [[ground truth|ground truth]].




