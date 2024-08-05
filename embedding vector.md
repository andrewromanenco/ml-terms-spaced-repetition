#language

Broadly speaking, an array of floating-point numbers taken from <strong>any</strong>
[[hidden layer|hidden layer]] that describe the inputs to that hidden layer.
Often, an embedding vector is the array of floating-point numbers trained in
an embedding layer. For example, suppose an embedding layer must learn an
embedding vector for each of the 73,000 tree species on Earth. Perhaps the
following array is the embedding vector for a baobab tree:


![[ images/EmbeddingBaobab.png ]]


An embedding vector is not a bunch of random numbers. An embedding layer
determines these values through training, similar to the way a
neural network learns other weights during training. Each element of the
array is a rating along some characteristic of a tree species. Which
element represents which tree species&#39; characteristic? That&#39;s very hard
for humans to determine.

The mathematically remarkable part of an embedding vector is that similar
items have similar sets of floating-point numbers. For example, similar
tree species have a more similar set of floating-point numbers than
dissimilar tree species. Redwoods and sequoias are related tree species,
so they&#39;ll have a more similar set of floating-pointing numbers than
redwoods and coconut palms. The numbers in the embedding vector will
change each time you retrain the model, even if you retrain the model
with identical input.

