
Reusing the [[example|examples]] of a [[minority class|minority class]]
in a [[class-imbalanced dataset|class-imbalanced dataset]] in order to
create a more balanced [[training set|training set]].

For example, consider a [[binary classification|binary classification]]
problem in which the ratio of the [[majority class|majority class]] to the
minority class is 5,000:1. If the dataset contains a million examples, then
the dataset contains only about 200 examples of the minority class, which might
be too few examples for effective training. To overcome this deficiency, you
might oversample (reuse) those 200 examples multiple times, possibly yielding
sufficient examples for useful training.

You need to be careful about over [[overfitting|overfitting]] when
oversampling.

Contrast with [[undersampling|undersampling]].


