#TensorFlow, #GoogleCloud

The process of [[inference|inferring]] predictions on multiple
[[unlabeled example|unlabeled examples]] divided into smaller
subsets (&quot;batches&quot;).

Batch inference can leverage the parallelization features of
[[accelerator chip|accelerator chips]]. That is, multiple accelerators
can simultaneously infer predictions on different batches of unlabeled
examples, dramatically increasing the number of inferences per second.

