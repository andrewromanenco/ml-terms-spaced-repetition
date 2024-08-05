#image

The following two-step mathematical operation:

<ol>
<li>Element-wise multiplication of the
[[convolutional filter|convolutional filter]] and a slice of an
input matrix. (The slice of the input matrix has the same rank and
size as the convolutional filter.)</li>
<li>Summation of all the values in the resulting product matrix.</li>
</ol>

For example, consider the following 5x5 input matrix:


![[ images/ConvolutionalLayerInputMatrix.svg ]]


Now imagine the following 2x2 convolutional filter:


![[ images/ConvolutionalLayerFilter.svg ]]


Each convolutional operation involves a single 2x2 slice of the
input matrix. For example, suppose we use the 2x2 slice at the
top-left of the input matrix. So, the convolution operation on
this slice looks as follows:


![[ images/ConvolutionalLayerOperation.svg ]]


A [[convolutional layer|convolutional layer]] consists of a
series of convolutional operations, each acting on a different slice
of the input matrix.

