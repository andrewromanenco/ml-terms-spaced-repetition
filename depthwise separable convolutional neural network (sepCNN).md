#image

A [[convolutional neural network|convolutional neural network]]
architecture based on
<a href="https://github.com/tensorflow/tpu/tree/master/models/experimental/inception">Inception</a>,
but where Inception modules are replaced with depthwise separable
convolutions. Also known as Xception.

A depthwise separable convolution (also abbreviated as separable convolution)
factors a standard 3D convolution into two separate convolution operations
that are more computationally efficient: first, a depthwise convolution,
with a depth of 1 (n ✕ n ✕ 1), and then second, a pointwise convolution,
with length and width of 1 (1 ✕ 1 ✕ n).

To learn more, see <a href="https://arxiv.org/pdf/1610.02357.pdf">Xception: Deep Learning with Depthwise Separable
Convolutions</a>.

