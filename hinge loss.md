
A family of [[loss|loss]] functions for
[[classification model|classification]] designed to find the
[[decision boundary|decision boundary]] as distant as possible
from each training example,
thus maximizing the margin between examples and the boundary.
[[Kernel Support Vector Machines (KSVMs)|KSVMs]] use hinge loss (or a related function, such as
squared hinge loss). For binary classification, the hinge loss function
is defined as follows:

<div>
$$\text{loss} = \text{max}(0, 1 - (y * y'))$$
</div>

where <em>y</em> is the true label, either -1 or +1, and <em>y&#39;</em> is the raw output
of the classifier model:

<div>
$$y' = b + w_1x_1 + w_2x_2 + … w_nx_n$$
</div>

Consequently, a plot of hinge loss versus (y * y&#39;) looks as follows:


![[ images/hinge-loss.svg ]]


