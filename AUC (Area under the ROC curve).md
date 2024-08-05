#fundamentals

A number between 0.0 and 1.0 representing a
[[binary classification|binary classification]] model&#39;s
ability to separate [[positive class|positive classes]] from
[[negative class|negative classes]].
The closer the AUC is to 1.0, the better the model&#39;s ability to separate
classes from each other.

For example, the following illustration shows a classifier model
that separates positive classes (green ovals) from negative classes
(purple rectangles) perfectly. This unrealistically perfect model has
an AUC of 1.0:


![[ images/AUCIdealClassSeparation.png ]]


Conversely, the following illustration shows the results for a classifier
model that generated random results. This model has an AUC of 0.5:


![[ images/AUCSetupPNPNPN.png ]]


Yes, the preceding model has an AUC of 0.5, not 0.0.

Most models are somewhere between the two extremes. For instance, the
following model separates positives from negatives somewhat, and therefore
has an AUC somewhere between 0.5 and 1.0:


![[ images/AUCSetupTypical.png ]]


AUC ignores any value you set for
[[classification threshold|classification threshold]]. Instead, AUC
considers <em>all</em> possible classification thresholds.

<section class="expandable">

<h4 class="showalways" id="click-the-icon-to-learn-about-the-relationship-between-auc-and-roc-curves." data-text=" Click the icon to learn about the relationship between AUC and ROC curves. " tabindex="-1">
Click the icon to learn about the relationship between AUC and ROC curves.
</h4>

<div class="expand-background">

AUC represents the <i>area</i> under an
<a href="#ROC"><b>ROC curve</b></a>.
For example,
the ROC curve for a model that perfectly separates positives from
negatives looks as follows:


![[ images/AUC1_0.png ]]


AUC is the area of the gray region in the preceding illustration.
In this unusual case, the area is simply the length of the gray region
(1.0) multiplied by the width of the gray region (1.0). So, the product
of 1.0 and 1.0 yields an AUC of exactly 1.0, which is the highest possible
AUC score.

Conversely, the ROC curve for a classifier that can't separate classes
at all is as follows. The area of this gray region is 0.5.


![[ images/AUC0_5.png ]]


A more typical ROC curve looks approximately like the following:


![[ images/ROCTypicalGraph.png ]]



It would be painstaking to calculate the area under this curve manually,
which is why a program typically calculates most AUC values.

</div>

<hr />
</section>

<section class="expandable">

<h4 class="showalways" id="click-the-icon-for-a-more-formal-definition-of-auc." data-text=" Click the icon for a more formal definition of AUC. " tabindex="-1">
Click the icon for a more formal definition of AUC.
</h4>

<div class="expand-background">

AUC is the probability that a classifier will be more confident that a
randomly chosen positive example is actually positive than that a
randomly chosen negative example is positive.


</div>

<hr />
</section>

