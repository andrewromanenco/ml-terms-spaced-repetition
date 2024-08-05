
In machine learning, a mechanism for bucketing
[[categorical data|categorical data]], particularly when the number
of categories is large, but the number of categories actually appearing
in the dataset is comparatively small.

For example, Earth is home to about 73,000 tree species. You could
represent each of the 73,000 tree species in 73,000 separate categorical
buckets. Alternatively, if only 200 of those tree species actually appear
in a dataset, you could use hashing to divide tree species into
perhaps 500 buckets.

A single bucket could contain multiple tree species. For example, hashing
could place <em>baobab</em> and <em>red maple</em>—two genetically dissimilar
species—into the same bucket. Regardless, hashing is still a good way to
map large categorical sets into the selected number of buckets. Hashing turns a
categorical feature having a large number of possible values into a much
smaller number of values by grouping values in a
deterministic way.

