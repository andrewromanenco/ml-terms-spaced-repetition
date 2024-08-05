
A [[backpropagation|backpropagation]] technique that updates the
[[parameter|parameters]] only <em>once per epoch</em> rather than once per
iteration. After processing each [[mini-batch|mini-batch]], gradient
accumulation simply updates a running total of gradients. Then, after
processing the last mini-batch in the epoch, the system finally updates
the parameters based on the total of all gradient changes.

Gradient accumulation is useful when the [[batch size|batch size]] is
very large compared to the amount of available memory for training.
When memory is an issue, the natural tendency is to reduce batch size.
However, reducing the batch size in normal backpropagation <em>increases</em>
the number of parameter updates. Gradient accumulation enables the model
to avoid memory issues but still train efficiently.

