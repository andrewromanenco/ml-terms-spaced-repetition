#language

A measurement of how similar two text strings are to each other.
In machine learning, edit distance is useful because it is simple to
compute, and an effective way to compare two strings that are known to be
similar or to find strings that are similar to a given string.

There are several definitions of edit distance, each using different string
operations. For example, the
<a href="https://wikipedia.org/wiki/Levenshtein_distance" target="T">
Levenshtein distance</a>
considers the fewest delete, insert, and substitute operations.

For example, the Levenshtein distance between the words &quot;heart&quot; and &quot;darts&quot;
is 3 because the following 3 edits are the fewest changes to turn one word
into the other:

<ol>
<li>heart → deart (substitute &quot;h&quot; with &quot;d&quot;)</li>
<li>deart → dart (delete &quot;e&quot;)</li>
<li>dart → darts (insert &quot;s&quot;)</li>
</ol>

