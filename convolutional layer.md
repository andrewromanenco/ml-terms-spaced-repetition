#image

A layer of a [[deep model|deep neural network]] in which a
[[convolutional filter|convolutional filter]] passes along an input
matrix. For example, consider the following 3x3
[[convolutional filter|convolutional filter]]:


![[ images/ConvolutionalFilter33.svg ]]


The following animation shows a convolutional layer consisting of 9
convolutional operations involving the 5x5 input matrix. Notice that each
convolutional operation works on a different 3x3 slice of the input matrix.
The resulting 3x3 matrix (on the right) consists of the results of the 9
convolutional operations:


![[ images/AnimatedConvolution.gif ]]


