#fundamentals

The number of [[example|examples]] in a [[batch|batch]].
For instance, if the batch size is 100, then the model processes
100 examples per [[iteration|iteration]].

The following are popular batch size strategies:

<ul>
<li>[[stochastic gradient descent (SGD)|Stochastic Gradient Descent (SGD)]], in which the batch size is 1.</li>
<li>Full batch, in which the batch size is the number of examples in the entire
[[training set|training set]]. For instance, if the training set
contains a million examples, then the batch size would be a million
examples. Full batch is usually an inefficient strategy.</li>
<li>[[mini-batch|mini-batch]] in which the batch size is usually between
10 and 1000. Mini-batch is usually the most efficient strategy.</li>
</ul>

