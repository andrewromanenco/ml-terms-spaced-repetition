#language

In [[language model|language models]], a [[token|token]] that is a
substring of a word, which may be the entire word.

For example, a word like &quot;itemize&quot; might be broken up into the pieces &quot;item&quot;
(a root word) and &quot;ize&quot; (a suffix), each of which is represented by its own
token. Splitting uncommon words into such pieces, called subwords, allows
language models to operate on the word&#39;s more common constituent parts,
such as prefixes and suffixes.

Conversely, common words like &quot;going&quot; might not be broken up and might be
represented by a single token.

