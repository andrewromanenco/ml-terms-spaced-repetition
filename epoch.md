#fundamentals

A full training pass over the entire [[training set|training set]]
such that each [[example|example]] has been processed once.

An epoch represents <code translate="no" dir="ltr">N</code>/[[batch size|batch size]]
training [[iteration|iterations]], where <code translate="no" dir="ltr">N</code> is the
total number of examples.

For instance, suppose the following:

<ul>
<li>The dataset consists of 1,000 examples.</li>
<li>The batch size is 50 examples.</li>
</ul>

Therefore, a single epoch requires 20 iterations:

<pre translate="no" dir="ltr">
1 epoch = (N/batch size) = (1,000 / 50) = 20 iterations
</pre>

