#language, #fundamentals

A [[feature|feature]] whose values are predominately zero or empty.
For example, a feature containing a single 1 value and a million 0 values is
sparse. In contrast, a [[dense feature|dense feature]] has values that
are predominantly not zero or empty.

In machine learning, a surprising number of features are sparse features.
Categorical features are usually sparse features.
For example, of the 300 possible tree species in a forest, a single example
might identify just a <em>maple tree</em>. Or, of the millions
of possible videos in a video library, a single example might identify
just &quot;Casablanca.&quot;

In a model, you typically represent sparse features with
[[one-hot encoding|one-hot encoding]]. If the one-hot encoding is big,
you might put an [[embedding layer|embedding layer]] on top of the
one-hot encoding for greater efficiency.

