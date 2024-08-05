#df

A mechanism for evaluating the quality of a
[[decision forest|decision forest]] by testing each
[[decision tree|decision tree]] against the
[[example|examples]] <em>not</em> used during
[[training|training]] of that decision tree. For example, in the
following diagram, notice that the system trains each decision tree
on about two-thirds of the examples and then evaluates against the
remaining one-third of the examples.


![[ images/OOBevaluation.png ]]


Out-of-bag evaluation is a computationally efficient and conservative
approximation of the [[cross-validation|cross-validation]] mechanism.
In cross-validation, one model is trained for each cross-validation round
(for example, 10 models are trained in a 10-fold cross-validation).
With OOB evaluation, a single model is trained. Because [[bagging|bagging]]
withholds some data from each tree during training, OOB evaluation can use
that data to approximate cross-validation.

