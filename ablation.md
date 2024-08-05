

A technique for evaluating the importance of a [[feature|feature]]
or component by temporarily <em>removing</em> it from a [[model|model]]. You then
retrain the model without that feature or component, and if the retrained model
performs significantly worse, then the removed feature or component was
likely important.

For example, suppose you train a
[[classification model|classification model]]
on 10 features and achieve 88% [[precision|precision]] on the
[[test set|test set]]. To check the [[variable importances|importance]]
of the first feature, you can retrain the model using only the nine other
features. If the retrained model performs significantly worse (for instance,
55% precision), then the removed feature was probably important. Conversely,
if the retrained model performs equally well, then that feature was probably
not that important.

Ablation can also help determine the importance of:

<ul>
<li>Larger components, such as an entire subsystem of a larger ML system</li>
<li>Processes or techniques, such as a data preprocessing step</li>
</ul>

In both cases, you would observe how the system&#39;s performance changes (or
doesn&#39;t change) after you&#39;ve removed the component.

