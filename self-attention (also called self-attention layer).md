#language

A neural network layer that transforms a sequence of
embeddings (for instance, [[token|token]] embeddings)
into another sequence of embeddings. Each embedding in the output sequence is
constructed by integrating information from the elements of the input sequence
through an [[attention|attention]] mechanism.

The <strong>self</strong> part of <strong>self-attention</strong> refers to the sequence attending to
itself rather than to some other context. Self-attention is one of the main
building blocks for [[Transformer|Transformers]] and uses dictionary lookup
terminology, such as &quot;query&quot;, &quot;key&quot;, and &quot;value&quot;.

A self-attention layer starts with a sequence of input representations, one
for each word. The input representation for a word can be a simple
embedding. For each word in an input sequence, the network
scores the relevance of the word to every element in the whole sequence of
words. The relevance scores determine how much the word&#39;s final representation
incorporates the representations of other words.

For example, consider the following sentence:

<blockquote>
The animal didn&#39;t cross the street because it was too tired.
</blockquote>

The following illustration (from
<a href="https://ai.googleblog.com/2017/08/transformer-novel-neural-network.html">Transformer: A Novel Neural Network Architecture for Language
Understanding</a>)
shows a self-attention layer&#39;s attention pattern for the pronoun <strong>it</strong>, with
the darkness of each line indicating how much each word contributes to the
representation:


![[ images/self-attention.png ]]


The self-attention layer highlights words that are relevant to &quot;it&quot;. In this
case, the attention layer has learned to highlight words that <strong>it</strong> might
refer to, assigning the highest weight to <strong>animal</strong>.

For a sequence of <em>n</em> [[token|tokens]], self-attention transforms a sequence
of embeddings <em>n</em> separate times, once at each position in the sequence.

Refer also to [[attention|attention]] and
[[multi-head self-attention|multi-head self-attention]].

