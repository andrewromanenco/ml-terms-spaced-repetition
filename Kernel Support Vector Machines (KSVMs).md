
A classification algorithm that seeks to maximize the margin between
[[positive class|positive]] and
[[negative class|negative classes]] by mapping input data vectors
to a higher dimensional space. For example, consider a classification
problem in which the input dataset
has a hundred features. To maximize the margin between
positive and negative classes, a KSVM could internally map those features into
a million-dimension space. KSVMs uses a loss function called
[[hinge loss|hinge loss]].

