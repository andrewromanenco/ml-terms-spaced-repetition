#image

Reducing a matrix (or matrixes) created by an earlier
[[convolutional layer|convolutional layer]] to a smaller matrix.
Pooling usually involves taking either the maximum or average value
across the pooled area. For example, suppose we have the
following 3x3 matrix:


![[ images/PoolingStart.svg ]]


A pooling operation, just like a convolutional operation, divides that
matrix into slices and then slides that convolutional operation by
[[stride|strides]]. For example, suppose the pooling operation
divides the convolutional matrix into 2x2 slices with a 1x1 stride.
As the following diagram illustrates, four pooling operations take place.
Imagine that each pooling operation picks the maximum value of the
four in that slice:


![[ images/PoolingConvolution.svg ]]


Pooling helps enforce
[[translational invariance|translational invariance]] in the input matrix.

Pooling for vision applications is known more formally as <strong>spatial pooling</strong>.
Time-series applications usually refer to pooling as <strong>temporal pooling</strong>.
Less formally, pooling is often called <strong>subsampling</strong> or <strong>downsampling</strong>.

