#image

In mathematics, casually speaking, a mixture of two functions. In machine
learning, a convolution mixes the [[convolutional filter|convolutional
filter]] and the input matrix
in order to train [[weight|weights]].

The term &quot;convolution&quot; in machine learning is often a shorthand way of
referring to either [[convolutional operation|convolutional operation]]
or [[convolutional layer|convolutional layer]].

Without convolutions, a machine learning algorithm would have to learn
a separate weight for every cell in a large [[Tensor|tensor]]. For example,
a machine learning algorithm training on 2K x 2K images would be forced to
find 4M separate weights. Thanks to convolutions, a machine learning
algorithm only has to find weights for every cell in the
[[convolutional filter|convolutional filter]], dramatically reducing
the memory needed to train the model. When the convolutional filter is
applied, it is simply replicated across cells such that each is multiplied
by the filter.

