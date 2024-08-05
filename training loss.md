#fundamentals

A [[metric|metric]] representing a model&#39;s [[loss|loss]] during a
particular training iteration. For example, suppose the loss function
is [[Mean Squared Error (MSE)|Mean Squared Error]]. Perhaps the training loss (the Mean
Squared Error) for the 10th iteration is 2.2, and the training loss for
the 100th iteration is 1.9.

A [[loss curve|loss curve]] plots training loss versus the number of
iterations. A loss curve provides the following hints about training:

<ul>
<li>A downward slope implies that the model is improving.</li>
<li>An upward slope implies that the model is getting worse.</li>
<li>A flat slope implies that the model has reached
[[convergence|convergence]].</li>
</ul>

For example, the following somewhat idealized [[loss curve|loss curve]]
shows:

<ul>
<li>A steep downward slope during the initial iterations, which implies
rapid model improvement.</li>
<li>A gradually flattening (but still downward) slope until close to the end
of training, which implies continued model improvement at a somewhat
slower pace then during the initial iterations.</li>
<li>A flat slope towards the end of training, which suggests convergence.</li>
</ul>


![[ images/TrainingLoss.png ]]


Although training loss is important, see also
[[generalization|generalization]].

