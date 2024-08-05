#df

In [[decision forest|decision forests]], the difference between
a node&#39;s [[entropy|entropy]] and the weighted (by number of examples)
sum of the entropy of its children nodes. A node&#39;s entropy is the entropy
of the examples in that node.

For example, consider the following entropy values:

<ul>
<li>entropy of parent node = 0.6</li>
<li>entropy of one child node with 16 relevant examples = 0.2</li>
<li>entropy of another child node with 24 relevant examples = 0.1</li>
</ul>

So 40% of the examples are in one child node and 60% are in the
other child node. Therefore:

<ul>
<li>weighted entropy sum of child nodes = (0.4 * 0.2) + (0.6 * 0.1) = 0.14</li>
</ul>

So, the information gain is:

<ul>
<li>information gain = entropy of parent node - weighted entropy sum of child nodes</li>
<li>information gain = 0.6 - 0.14 = 0.46</li>
</ul>

Most [[splitter|splitters]] seek to create [[condition|conditions]]
that maximize information gain.

