#fundamentals

A single update of a [[model|model&#39;s]] parameters—the model&#39;s
[[weight|weights]] and [[bias (math) or bias term|biases]]—during
[[training|training]]. The [[batch size|batch size]] determines
how many examples the model processes in a single iteration. For instance,
if the batch size is 20, then the model processes 20 examples before
adjusting the parameters.

When training a [[neural network|neural network]], a single iteration
involves the following two passes:

<ol>
<li>A forward pass to evaluate loss on a single batch.</li>
<li>A backward pass ([[backpropagation|backpropagation]]) to adjust the
model&#39;s parameters based on the loss and the learning rate.</li>
</ol>


