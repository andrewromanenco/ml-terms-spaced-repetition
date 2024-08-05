
A subset of the [[data set or dataset|dataset]] reserved for testing
a trained [[model|model]].

Traditionally, you divide examples in the dataset into the following three
distinct subsets:

<ul>
<li>a [[training set|training set]]</li>
<li>a [[validation set|validation set]]</li>
<li>a test set</li>
</ul>

Each example in a dataset should belong to only one of the preceding subsets.
For instance, a single example shouldn&#39;t belong to both the training set and
the test set.

The training set and validation set are both closely tied to training a model.
Because the test set is only indirectly associated with training,
[[test loss|test loss]] is a less biased, higher quality metric than
[[training loss|training loss]] or [[validation loss|validation loss]].



