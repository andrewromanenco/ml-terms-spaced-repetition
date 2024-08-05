
A copy of the [[training set|training set]] or [[model|model]],
typically on another machine. For example, a system could use the following
strategy for implementing [[data parallelism|data parallelism]]:

<ol>
<li>Place replicas of an existing model on multiple machines.</li>
<li>Send different subsets of the training set to each replica.</li>
<li>Aggregate the [[parameter|parameter]] updates.</li>
</ol>

