
The vector of raw (non-normalized) predictions that a classification
model generates, which is ordinarily then passed to a normalization function.
If the model is solving a [[multi-class classification|multi-class classification]]
problem, logits typically become an input to the
[[softmax|softmax]] function.
The softmax function then generates a vector of (normalized)
probabilities with one value for each possible class.

