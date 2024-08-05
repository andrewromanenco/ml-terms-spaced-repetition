
Very overloaded term whose meaning varies across different mathematical
and scientific fields. Within machine learning, a vector has two properties:

<ul>
<li>Data type: Vectors in machine learning usually hold floating-point numbers.</li>
<li>Number of elements: This is the vector&#39;s length or its <em>dimension</em>.</li>
</ul>

For example, consider a [[feature vector|feature vector]] that holds eight
floating-point numbers. This feature vector has a length or dimension of eight.
Note that machine learning vectors often have a huge number of dimensions.

You can represent many different kinds of information as a vector. For example:

<ul>
<li>Any position on the surface of Earth can be represented as a 2-dimensional
vector, where one dimension is the latitude and the other is the longitude.</li>
<li>The current prices of each of 500 stocks can be represented as a
500-dimensional vector.</li>
<li>A probability distribution over a finite number of classes can be represented
as a vector. For example, a
[[multi-class classification|multiclass classification]] system that
predicts one of three output colors (red, green, or yellow) could output the
vector <code translate="no" dir="ltr">(0.3, 0.2, 0.5)</code> to mean <code translate="no" dir="ltr">P[red]=0.3, P[green]=0.2, P[yellow]=0.5</code>.</li>
</ul>

Vectors can be concatenated; therefore, a variety of different media can be
represented as a single vector. Some models operate directly on the
concatenation of many [[one-hot encoding|one-hot encodings]].

Specialized processors such as [[TPU|TPUs]] are optimized to perform
mathematical operations on vectors.

A vector is a [[Tensor|tensor]] of [[rank (ordinality)|rank]] 1.




