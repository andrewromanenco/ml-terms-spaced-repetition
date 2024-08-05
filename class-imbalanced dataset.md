#fundamentals

A dataset for a classification problem in which the total number
of [[label|labels]] of each class differs significantly.
For example, consider a binary classification dataset whose two labels
are divided as follows:

<ul>
<li>1,000,000 negative labels</li>
<li>10 positive labels</li>
</ul>

The ratio of negative to positive labels is 100,000 to 1, so this
is a class-imbalanced dataset.

In contrast, the following dataset is <em>not</em> class-imbalanced because the
ratio of negative labels to positive labels is relatively close to 1:

<ul>
<li>517 negative labels</li>
<li>483 positive labels</li>
</ul>

Multi-class datasets can also be class-imbalanced. For example, the following
multi-class classification dataset is also class-imbalanced because one label
has far more examples than the other two:

<ul>
<li>1,000,000 labels with class &quot;green&quot;</li>
<li>200 labels with class &quot;purple&quot;</li>
<li>350 labels with class &quot;orange&quot;</li>
</ul>

See also [[entropy|entropy]], [[majority class|majority class]],
and [[minority class|minority class]].

