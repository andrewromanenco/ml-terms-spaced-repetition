#language

Dividing a sentence into smaller grammatical structures (&quot;constituents&quot;).
A later part of the ML system, such as a
[[natural language understanding|natural language understanding]] model,
can parse the constituents more easily than the original sentence. For example,
consider the following sentence:

<blockquote>
My friend adopted two cats.
</blockquote>

A constituency parser can divide this sentence into the following
two constituents:

<ul>
<li><em>My friend</em> is a noun phrase.</li>
<li><em>adopted two cats</em> is a verb phrase.</li>
</ul>

These constituents can be further subdivided into smaller constituents.
For example, the verb phrase

<blockquote>
adopted two cats
</blockquote>

could be further subdivided into:

<ul>
<li><em>adopted</em> is a verb.</li>
<li><em>two cats</em> is another noun phrase.</li>
</ul>

