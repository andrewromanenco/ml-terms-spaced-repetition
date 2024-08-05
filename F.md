
A &quot;roll-up&quot; [[binary classification|binary classification]] metric that
relies on both [[precision|precision]] and [[recall|recall]].
Here is the formula:

<div>
$$F{_1} =
\frac{\text{2 * precision * recall}} {\text{precision + recall}}$$
</div>

For example, given the following:

<ul>
<li>precision = 0.6</li>
<li>recall = 0.4</li>
</ul>

<div>
$$F{_1} =
\frac{\text{2 * 0.6 * 0.4}} {\text{0.6 + 0.4}} = 0.48$$
</div>

When precision and recall are fairly similar (as in the preceding example),
F<sub>1</sub> is close to their mean. When precision and recall differ
significantly, F<sub>1</sub> is closer to the lower value. For example:

<ul>
<li>precision = 0.9</li>
<li>recall = 0.1</li>
</ul>

<div>
$$F{_1} =
\frac{\text{2 * 0.9 * 0.1}} {\text{0.9 + 0.1}} = 0.18$$
</div>

