#fundamentals

A graph of [[true positive rate (TPR)|true positive rate]] versus
[[false positive rate (FPR)|false positive rate]] for different
[[classification threshold|classification thresholds]] in binary
classification.

The shape of an ROC curve suggests a binary classification model&#39;s ability
to separate positive classes from negative classes. Suppose, for example,
that a binary classification model perfectly separates all the negative
classes from all the positive classes:


![[ images/ROCSetupIdealDistributionNoClassificationThreshold.png ]]


The ROC curve for the preceding model looks as follows:


![[ images/ROCcurvePerfect.png ]]


In contrast, the following illustration graphs the raw logistic regression
values for a terrible model that can&#39;t separate negative classes from
positive classes at all:


![[ images/ROCWorstCaseDistribution.png ]]


The ROC curve for this model looks as follows:


![[ images/ROCcurveWorstCase.png ]]


Meanwhile, back in the real world, most binary classification models separate
positive and negative classes to some degree, but usually not perfectly. So,
a typical ROC curve falls somewhere between the two extremes:


![[ images/ROCTypicalGraph.png ]]


The point on an ROC curve closest to (0.0,1.0) theoretically identifies the
ideal classification threshold. However, several other real-world issues
influence the selection of the ideal classification threshold. For example,
perhaps false negatives cause far more pain than false positives.

A numerical metric called [[AUC (Area under the ROC curve)|AUC]] summarizes the ROC curve into
a single floating-point value.

