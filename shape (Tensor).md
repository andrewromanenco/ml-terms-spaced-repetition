

The number of elements in each <b><a href="#dimensions">dimension</a></b> of a
tensor. The shape is represented as a list of integers. For example,
the following two-dimensional tensor has a shape of [3,4]:


<pre class="prettyprint" translate="no" dir="ltr">
[[5, 7, 6, 4],
 [2, 9, 4, 8],
 [3, 6, 5, 1]]
</pre>

TensorFlow uses row-major (C-style) format to represent the order of
dimensions, which is why the shape in TensorFlow is <code translate="no" dir="ltr">[3,4]</code> rather than
<code translate="no" dir="ltr">[4,3]</code>. In other words, in a two-dimensional TensorFlow Tensor, the shape
is <code translate="no" dir="ltr">[</code><em>number of rows</em>, <em>number of columns</em><code translate="no" dir="ltr">]</code>.

A <strong>static shape</strong> is a tensor shape that is <em>known</em> at compile time.

A <strong>dynamic shape</strong> is <em>unknown</em> at compile time and is
therefore dependent on runtime data. This tensor might be represented with a
placeholder dimension in TensorFlow, as in <code translate="no" dir="ltr">[3, ?]</code>.

