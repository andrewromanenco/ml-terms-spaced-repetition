#fundamentals

A [[synthetic feature|synthetic feature]] formed by &quot;crossing&quot;
[[categorical data|categorical]] or [[bucketing|bucketed]] features.

For example, consider a &quot;mood forecasting&quot; model that represents
temperature in one of the following four buckets:

<ul>
<li><code translate="no" dir="ltr">freezing</code></li>
<li><code translate="no" dir="ltr">chilly</code></li>
<li><code translate="no" dir="ltr">temperate</code></li>
<li><code translate="no" dir="ltr">warm</code></li>
</ul>

And represents wind speed in one of the following three buckets:

<ul>
<li><code translate="no" dir="ltr">still</code></li>
<li><code translate="no" dir="ltr">light</code></li>
<li><code translate="no" dir="ltr">windy</code></li>
</ul>

Without feature crosses, the linear model trains independently on each of the
preceding seven various buckets. So, the model trains on, for instance,
<code translate="no" dir="ltr">freezing</code> independently of the training on, for instance,
<code translate="no" dir="ltr">windy</code>.

Alternatively, you could create a feature cross of temperature and
wind speed. This synthetic feature would have the following 12 possible
values:

<ul>
<li><code translate="no" dir="ltr">freezing-still</code></li>
<li><code translate="no" dir="ltr">freezing-light</code></li>
<li><code translate="no" dir="ltr">freezing-windy</code></li>
<li><code translate="no" dir="ltr">chilly-still</code></li>
<li><code translate="no" dir="ltr">chilly-light</code></li>
<li><code translate="no" dir="ltr">chilly-windy</code></li>
<li><code translate="no" dir="ltr">temperate-still</code></li>
<li><code translate="no" dir="ltr">temperate-light</code></li>
<li><code translate="no" dir="ltr">temperate-windy</code></li>
<li><code translate="no" dir="ltr">warm-still</code></li>
<li><code translate="no" dir="ltr">warm-light</code></li>
<li><code translate="no" dir="ltr">warm-windy</code></li>
</ul>

Thanks to feature crosses, the model can learn mood differences
between a <code translate="no" dir="ltr">freezing-windy</code> day and a <code translate="no" dir="ltr">freezing-still</code> day.

If you create a synthetic feature from two features that each have a lot of
different buckets, the resulting feature cross will have a huge number
of possible combinations. For example, if one feature has 1,000 buckets and
the other feature has 2,000 buckets, the resulting feature cross has 2,000,000
buckets.

Formally, a cross is a
<a href="https://wikipedia.org/wiki/Cartesian_product" target="T">Cartesian product</a>.

Feature crosses are mostly used with linear models and are rarely used
with neural networks.

