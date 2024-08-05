#language, #fundamentals

A special [[hidden layer|hidden layer]] that trains on a
high-dimensional [[categorical data|categorical]] feature to
gradually learn a lower dimension embedding vector. An
embedding layer enables a neural network to train far more
efficiently than training just on the high-dimensional categorical feature.

For example, Earth currently supports about 73,000 tree species. Suppose
tree species is a [[feature|feature]] in your model, so your model&#39;s
input layer includes a [[one-hot encoding|one-hot vector]] 73,000
elements long.
For example, perhaps <code translate="no" dir="ltr">baobab</code> would be represented something like this:


![[ images/One-HotRepresentationOfTreeSpecies.png ]]


A 73,000-element array is very long. If you don&#39;t add an embedding layer
to the model, training is going to be very time consuming due to
multiplying 72,999 zeros. Perhaps you pick the embedding layer to consist
of 12 dimensions. Consequently, the embedding layer will gradually learn
a new embedding vector for each tree species.

In certain situations, [[hashing|hashing]] is a reasonable alternative
to an embedding layer.

