
A single number or a single string that can be represented as a
[[Tensor|tensor]] of [[rank (ordinality)|rank]] 0. For example, the following
lines of code each create one scalar in TensorFlow:

<pre class="prettyprint" translate="no" dir="ltr">
breed = tf.Variable("poodle", tf.string)
temperature = tf.Variable(27, tf.int16)
precision = tf.Variable(0.982375101275, tf.float64)
</pre>

