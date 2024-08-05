
A training-time optimization that calculates a probability for all the
[[positive class|positive]] labels, using, for example,
[[softmax|softmax]], but only for a random
sample of negative labels. For instance, given an example labeled
<em>beagle</em> and <em>dog</em>, candidate sampling computes the predicted probabilities
and corresponding loss terms for:

<ul>
<li><em>beagle</em></li>
<li><em>dog</em></li>
<li>a random subset of the remaining negative classes (for example, <em>cat</em>,
<em>lollipop</em>, <em>fence</em>).</li>
</ul>

The idea is that the
[[negative class|negative classes]] can learn from less frequent
negative reinforcement as long as
[[positive class|positive classes]] always get proper positive
reinforcement, and this is indeed observed empirically.

Candidate sampling is more computationally efficient than training algorithms
that compute predictions for <em>all</em> negative classes, particularly when the
number of negative classes is very large.

