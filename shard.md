#TensorFlow, #GoogleCloud

A logical division of the [[training set|training set]] or the
[[model|model]]. Typically, some process creates shards by dividing
the [[example|examples]] or [[parameter|parameters]] into (usually)
equal-sized chunks. Each shard is then assigned to a different machine.

Sharding a model is called [[model parallelism|model parallelism]];
sharding data is called [[data parallelism|data parallelism]].

