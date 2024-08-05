#language

A representation of the words in a phrase or passage,
irrespective of order. For example, bag of words represents the
following three phrases identically:

<ul>
<li>the dog jumps</li>
<li>jumps the dog</li>
<li>dog jumps the</li>
</ul>

Each word is mapped to an index in a [[sparse vector|sparse vector]], where
the vector has an index for every word in the vocabulary. For example,
the phrase <em>the dog jumps</em> is mapped into a feature vector with non-zero
values at the three indexes corresponding to the words <em>the</em>, <em>dog</em>, and
<em>jumps</em>. The non-zero value can be any of the following:

<ul>
<li>A 1 to indicate the presence of a word.</li>
<li>A count of the number of times a word appears in the bag. For example,
if the phrase were <em>the maroon dog is a dog with maroon fur</em>, then both
<em>maroon</em> and <em>dog</em> would be represented as 2, while the other words would
be represented as 1.</li>
<li>Some other value, such as the logarithm of the count of the number of
times a word appears in the bag.</li>
</ul>

