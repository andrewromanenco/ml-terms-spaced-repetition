#fundamentals

The array of [[feature|feature]] values comprising an
[[example|example]]. The feature vector is input during
[[training|training]] and during [[inference|inference]].
For example, the feature vector for a model with two discrete features
might be:

<pre class="prettyprint" translate="no" dir="ltr">
[0.92, 0.56]
</pre>


![[ images/FeatureVector.png ]]


Each example supplies different values for the feature vector, so the
feature vector for the next example could be something like:

<pre class="prettyprint" translate="no" dir="ltr">
[0.73, 0.49]
</pre>

[[feature engineering|Feature engineering]] determines how to represent
features in the feature vector. For example, a binary categorical feature with
five possible values might be represented with
[[one-hot encoding|one-hot encoding]]. In this case, the portion of the
feature vector for a particular example would consist of four zeroes and
a single 1.0 in the third position, as follows:

<pre translate="no" dir="ltr">
[0.0, 0.0, 1.0, 0.0, 0.0]
</pre>

As another example, suppose your model consists of three features:

<ul>
<li>a binary categorical feature with <em>five</em> possible values represented with
one-hot encoding; for example: <code translate="no" dir="ltr">[0.0, 1.0, 0.0, 0.0, 0.0]</code></li>
<li>another binary categorical feature with <em>three</em> possible values represented
with one-hot encoding; for example: <code translate="no" dir="ltr">[0.0, 0.0, 1.0]</code></li>
<li>a floating-point feature; for example: <code translate="no" dir="ltr">8.3</code>.</li>
</ul>

In this case, the feature vector for each example would be represented
by <em>nine</em> values. Given the example values in the preceding list, the
feature vector would be:

<pre translate="no" dir="ltr">
0.0
1.0
0.0
0.0
0.0
0.0
0.0
1.0
8.3
</pre>

