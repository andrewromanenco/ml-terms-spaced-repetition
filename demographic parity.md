#fairness

A [[fairness metric|fairness metric]] that is satisfied if
the results of a model&#39;s classification are not dependent on a
given [[sensitive attribute|sensitive attribute]].

For example, if both Lilliputians and Brobdingnagians apply to
Glubbdubdrib University, demographic parity is achieved if the percentage
of Lilliputians admitted is the same as the percentage of Brobdingnagians
admitted, irrespective of whether one group is on average more qualified
than the other.

Contrast with [[equalized odds|equalized odds]] and
[[equality of opportunity|equality of opportunity]], which permit
classification results in aggregate to depend on sensitive attributes,
but don&#39;t permit classification results for certain specified
[[ground truth|ground truth]] labels to depend on sensitive attributes. See
<a href="http://research.google.com/bigpicture/attacking-discrimination-in-ml/"
target="T">&quot;Attacking
discrimination with smarter machine learning&quot;</a> for a visualization
exploring the tradeoffs when optimizing for demographic parity.

