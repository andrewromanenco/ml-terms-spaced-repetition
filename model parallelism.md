#language

A way of scaling training or inference that puts different parts of one
[[model|model]] on different [[device|devices]]. Model parallelism
enables models that are too big to fit on a single device.

To implement model parallelism, a system typically does the following:

<ol>
<li>Shards (divides) the model into smaller parts.</li>
<li>Distributes the training of those smaller parts across multiple processors.
Each processor trains its own part of the model.</li>
<li>Combines the results to create a single model.</li>
</ol>

Model parallelism slows training.



See also [[data parallelism|data parallelism]].

