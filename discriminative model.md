
A [[model|model]] that predicts [[label|labels]] from a set of one or
more [[feature|features]]. More formally, discriminative models define the
conditional probability of an output given the features and
[[weight|weights]]; that is:

<pre class="prettyprint" translate="no" dir="ltr">
p(output | features, weights)
</pre>

For example, a model that predicts whether an email is spam from features
and weights is a discriminative model.

The vast majority of supervised learning models, including classification
and regression models, are discriminative models.

Contrast with [[generative model|generative model]].

