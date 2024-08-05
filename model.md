#fundamentals

In general, any mathematical construct that processes input data and returns
output. Phrased differently, a model is the set of parameters and structure
needed for a system to make predictions.
In [[supervised machine learning|supervised machine learning]],
a model takes an [[example|example]] as input and infers a
[[prediction|prediction]] as output. Within supervised machine learning,
models differ somewhat. For example:

<ul>
<li>A linear regression model consists of a set of [[weight|weights]]
and a [[bias (math) or bias term|bias]].</li>
<li>A [[neural network|neural network]] model consists of:
<ul>
<li>A set of [[hidden layer|hidden layers]], each containing one or
more [[neuron|neurons]].</li>
<li>The weights and bias associated with each neuron.</li>
</ul></li>
<li>A [[decision tree|decision tree]] model consists of:
<ul>
<li>The shape of the tree; that is, the pattern in which the conditions
and leaves are connected.</li>
<li>The conditions and leaves.</li>
</ul></li>
</ul>

You can save, restore, or make copies of a model.

[[unsupervised machine learning|Unsupervised machine learning]] also
generates models, typically a function that can map an input example to
the most appropriate [[clustering|cluster]].

<section class="expandable">

<h4 class="showalways" id="click-the-icon-to-compare-algebraic-and-programming-functions-to-ml-models." data-text=" Click the icon to compare algebraic and programming functions to ML models. " tabindex="-1">
Click the icon to compare algebraic and programming functions to ML models.
</h4>

<div class="expand-background">
An algebraic function such as the following is a model:

<pre translate="no" dir="ltr">
  f(x, y) = 3x -5xy + y<sup>2</sup> + 17
</pre>

The preceding function maps input values (<tt>x</tt> and <tt>y</tt>) to
output.

Similarly, a programming function like the following is also a model:

<pre class="prettyprint" translate="no" dir="ltr">
def half_of_greater(x, y):
  if (x > y):
    return(x / 2)
  else
    return(y / 2)
</pre>

A caller passes arguments to the preceding Python function, and the
Python function generates output (via the <tt>return</tt> statement).

Although a <a href="#deep_neural_network"><b>deep neural network</b></a>
has a very different mathematical structure than an algebraic or programming
function, a deep neural network still takes input (an example) and returns
output (a prediction).

A human programmer codes a programming function manually. In contrast,
a machine learning model gradually learns the optimal parameters
during automated training.

</div>

<hr />
</section>

