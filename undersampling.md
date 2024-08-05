
Removing [[example|examples]] from the
[[majority class|majority class]] in a
[[class-imbalanced dataset|class-imbalanced dataset]] in order to
create a more balanced [[training set|training set]].

For example, consider a dataset in which the ratio of the majority class to
the [[minority class|minority class]] is 20:1. To overcome this class
imbalance, you could create a training set consisting of <em>all</em> of the minority
class examples but only a <em>tenth</em> of the majority class examples, which would
create a training-set class ratio of 2:1. Thanks to undersampling, this more
balanced training set might produce a better model. Alternatively, this
more balanced training set might contain insufficient examples to train an
effective model.

Contrast with [[oversampling|oversampling]].

