#image

In a convolutional operation or pooling, the delta in each dimension of the
next series of input slices. For example, the following animation
demonstrates a (1,1) stride during a convolutional operation. Therefore,
the next input slice starts one position to the right of the previous input
slice. When the operation reaches the right edge, the next slice is all
the way over to the left but one position down.


![[ images/AnimatedConvolution.gif ]]


The preceding example demonstrates a two-dimensional stride. If the input
matrix is three-dimensional, the stride would also be three-dimensional.

