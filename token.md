#language

In a [[language model|language model]], the atomic unit that the model is
training on and making predictions on. A token is typically one of the
following:

<ul>
<li>a word—for example, the phrase &quot;dogs like cats&quot; consists of three word
tokens: &quot;dogs&quot;, &quot;like&quot;, and &quot;cats&quot;.</li>
<li>a character—for example, the phrase &quot;bike fish&quot; consists of nine
character tokens. (Note that the blank space counts as one of the tokens.)</li>
<li>subwords—in which a single word can be a single token or multiple tokens.
A subword consists of a root word, a prefix, or a suffix. For example,
a language model that uses subwords as tokens might view the word &quot;dogs&quot;
as two tokens (the root word &quot;dog&quot; and the plural suffix &quot;s&quot;). That same
language model might view the single word &quot;taller&quot; as two subwords (the
root word &quot;tall&quot; and the suffix &quot;er&quot;).</li>
</ul>

In domains outside of language models, tokens can represent other kinds of
atomic units. For example, in computer vision, a token might be a subset
of an image.

