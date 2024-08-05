#fundamentals

During [[training|training]] or testing, a
mathematical function that calculates the
loss on a [[batch|batch]] of examples. A loss function returns a lower loss
for models that makes good predictions than for models that make
bad predictions.

The goal of training is typically to minimize the loss that a loss function
returns.

Many different kinds of loss functions exist. Pick the appropriate loss
function for the kind of model you are building. For example:

<ul>
<li><a href="#L2_loss"><strong>L<sub>2</sub> loss</strong></a> (or [[Mean Squared Error (MSE)|Mean Squared Error]])
is the loss function for [[linear regression|linear regression]].</li>
<li>[[Log Loss|Log Loss]] is the loss function for
[[logistic regression|logistic regression]].</li>
</ul>

