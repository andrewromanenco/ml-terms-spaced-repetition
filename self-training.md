
A variant of [[self-supervised learning|self-supervised learning]] that is
particularly useful when all of the following conditions are true:

<ul>
<li>The ratio of [[unlabeled example|unlabeled examples]] to
[[labeled example|labeled examples]] in the dataset is high.</li>
<li>This is a [[classification model|classification]] problem.</li>
</ul>

Self-training works by iterating over the following two steps until the model
stops improving:

<ol>
<li>Use [[supervised machine learning|supervised machine learning]] to
 train a model on the labeled examples.</li>
<li>Use the model created in Step 1 to generate predictions (labels) on the
 unlabeled examples, moving those in which there is high confidence into
 the labeled examples with the predicted label.</li>
</ol>

Notice that each iteration of Step 2 adds more labeled examples for Step 1 to
train on.

