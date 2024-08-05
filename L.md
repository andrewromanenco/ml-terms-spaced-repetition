#fundamentals

A type of [[regularization|regularization]] that penalizes
[[weight|weights]] in proportion to the sum of the <em>squares</em> of the weights.
L<sub>2</sub> regularization helps drive [[outliers|outlier]] weights (those
with high positive or low negative values) closer to 0 but <em>not quite to 0</em>.
Features with values very close to 0 remain in the model
but don&#39;t influence the model&#39;s prediction very much.

L<sub>2</sub> regularization always improves generalization in
[[linear model|linear models]].

Contrast with <a href="#L1_regularization"><strong>L<sub>1</sub> regularization</strong></a>.

