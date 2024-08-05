#image

Artificially boosting the range and number of
[[training|training]] examples
by transforming existing
[[example|examples]] to create additional examples. For example,
suppose images are one of your
[[feature|features]], but your dataset doesn&#39;t
contain enough image examples for the model to learn useful associations.
Ideally, you&#39;d add enough
[[label|labeled]] images to your dataset to
enable your model to train properly. If that&#39;s not possible, data augmentation
can rotate, stretch, and reflect each image to produce many variants of the
original picture, possibly yielding enough labeled data to enable excellent
training.

