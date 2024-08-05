
Practically speaking, a model that does either of the following:

<ul>
<li>Creates (generates) new examples from the training dataset.
For example, a generative model could create poetry after training
on a dataset of poems. The [[generator|generator]] part of a
[[generative adversarial network (GAN)|generative adversarial network]]
falls into this category.</li>
<li>Determines the probability that a new example comes from the
training set, or was created from the same mechanism that created
the training set. For example, after training on
a dataset consisting of English sentences, a generative model could
determine the probability that new input is a valid English sentence.</li>
</ul>

A generative model can theoretically discern the distribution of examples
or particular features in a dataset. That is:

<pre class="prettyprint" translate="no" dir="ltr">
p(examples)
</pre>

Unsupervised learning models are generative.

Contrast with [[discriminative model|discriminative models]].

