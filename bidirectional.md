#language

A term used to describe a system that evaluates the text that both <em>precedes</em>
and <em>follows</em> a target section of text. In contrast, a
[[unidirectional|unidirectional]] system only
evaluates the text that <em>precedes</em> a target section of text.

For example, consider a [[masked language model|masked language model]] that
must determine probabilities for the word or words representing the underline in
the following question:

<blockquote>
What is the _____ with you?
</blockquote>

A unidirectional language model would have to base its probabilities only
on the context provided by the words &quot;What&quot;, &quot;is&quot;, and &quot;the&quot;. In contrast,
a bidirectional language model could also gain context from &quot;with&quot; and &quot;you&quot;,
which might help the model generate better predictions.

