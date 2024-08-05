
Values distant from most other values. In machine learning, any of the
following are outliers:

<ul>
<li>Input data whose values are more than roughly 3 standard deviations
from the mean.</li>
<li>[[weight|Weights]] with high absolute values.</li>
<li>Predicted values relatively far away from the actual values.</li>
</ul>

For example, suppose that <code translate="no" dir="ltr">widget-price</code> is a feature of a certain model.
Assume that the mean <code translate="no" dir="ltr">widget-price</code> is 7 Euros with a standard deviation
of 1 Euro. Examples containing a <code translate="no" dir="ltr">widget-price</code> of 12 Euros or 2 Euros
would therefore be considered outliers because each of those prices is
five standard deviations from the mean.

Outliers are often caused by typos or other input mistakes. In other cases,
outliers aren&#39;t mistakes; after all, values five standard deviations away
from the mean are rare but hardly impossible.

Outliers often cause problems in model training. [[clipping|Clipping]]
is one way of managing outliers.

