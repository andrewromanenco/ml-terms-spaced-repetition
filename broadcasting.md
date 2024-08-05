
Expanding the shape of an operand in a matrix math operation to
[[dimensions|dimensions]] compatible for that operation. For example,
linear algebra requires that the two operands in a matrix addition operation
must have the same dimensions. Consequently, you can&#39;t add a matrix of shape
(m, n) to a vector of length n. Broadcasting enables this operation by
virtually expanding the vector of length n to a matrix of shape (m, n) by
replicating the same values down each column.

For example, given the following definitions, linear algebra prohibits
A+B because A and B have different dimensions:
<pre class="prettyprint" translate="no" dir="ltr"><code translate="no" dir="ltr">A = [[7, 10, 4],
     [13, 5, 9]]
B = [2]
</code></pre>
However, broadcasting enables the operation A+B by virtually expanding B to:
<pre class="prettyprint" translate="no" dir="ltr"><code translate="no" dir="ltr"> [[2, 2, 2],
  [2, 2, 2]]
</code></pre>
Thus, A+B is now a valid operation:
<pre class="prettyprint" translate="no" dir="ltr"><code translate="no" dir="ltr">[[7, 10, 4],  +  [[2, 2, 2],  =  [[ 9, 12, 6],
 [13, 5, 9]]      [2, 2, 2]]      [15, 7, 11]]
</code></pre>
See the following description of
<a href="https://docs.scipy.org/doc/numpy-1.15.0/user/basics.broadcasting.html"
target="T">broadcasting in NumPy</a> for more details.

