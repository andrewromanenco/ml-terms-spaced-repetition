#fairness, #fundamentals

Adjusting the output of a model <em>after</em> the model has been run.
Post-processing can be used to enforce fairness constraints without
modifying models themselves.

For example, one might apply post-processing to a binary classifier
by setting a classification threshold such that
[[equality of opportunity|equality of opportunity]] is maintained
for some attribute by checking that the [[true positive rate (TPR)|true positive rate]]
is the same for all values of that attribute.

<a class="glossary-anchor" name="PR_AUC"></a>
<a class="glossary-anchor" name="area_under_the_pr_curve"></a>
