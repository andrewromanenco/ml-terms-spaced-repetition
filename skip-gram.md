#language

An [[N-gram|n-gram]] which may omit (or &quot;skip&quot;) words from the original
context, meaning the N words might not have been originally adjacent. More
precisely, a &quot;k-skip-n-gram&quot; is an n-gram for which up to k words may have
been skipped.

For example, &quot;the quick brown fox&quot; has the following possible 2-grams:

<ul>
<li>&quot;the quick&quot;</li>
<li>&quot;quick brown&quot;</li>
<li>&quot;brown fox&quot;</li>
</ul>

A &quot;1-skip-2-gram&quot; is a pair of words that have at most 1 word between them.
Therefore, &quot;the quick brown fox&quot; has the following 1-skip 2-grams:

<ul>
<li>&quot;the brown&quot;</li>
<li>&quot;quick fox&quot;</li>
</ul>

In addition, all the 2-grams are <em>also</em> 1-skip-2-grams, since fewer
than one word may be skipped.

Skip-grams are useful for understanding more of a word&#39;s surrounding context.
In the example, &quot;fox&quot; was directly associated with &quot;quick&quot; in the set of
1-skip-2-grams, but not in the set of 2-grams.

Skip-grams help train
<a href="/machine-learning/glossary#word-embedding"><strong>word embedding</strong></a> models.

