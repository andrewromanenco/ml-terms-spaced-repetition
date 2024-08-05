#fundamentals

A small, randomly selected subset of a [[batch|batch]] processed in one
[[iteration|iteration]].
The [[batch size|batch size]] of a mini-batch is usually
between 10 and 1,000 examples.

For example, suppose the entire training set (the full batch)
consists of 1,000 examples. Further suppose that you set the
[[batch size|batch size]] of each mini-batch to 20. Therefore, each
iteration determines the loss on a random 20 of the 1,000 examples and then
adjusts the [[weight|weights]] and [[bias (math) or bias term|biases]] accordingly.

It is much more efficient to calculate the loss on a mini-batch than the
loss on all the examples in the full batch.

