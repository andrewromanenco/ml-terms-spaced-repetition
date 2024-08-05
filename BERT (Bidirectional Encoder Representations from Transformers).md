#language

A model architecture for text [[representation|representation]]. A trained
BERT model can act as part of a larger model for text classification or
other ML tasks.

BERT has the following characteristics:

<ul>
<li>Uses the [[Transformer|Transformer]] architecture, and therefore relies
on [[self-attention (also called self-attention layer)|self-attention]].</li>
<li>Uses the [[encoder|encoder]] part of the Transformer. The encoder&#39;s job
is to produce good text representations, rather than to perform a specific
task like classification.</li>
<li>Is [[bidirectional|bidirectional]].</li>
<li>Uses [[masked language model|masking]] for
[[unsupervised machine learning|unsupervised training]].</li>
</ul>

BERT&#39;s variants include:

<ul>
<li><a href="https://ai.googleblog.com/2019/12/albert-lite-bert-for-self-supervised.html">ALBERT</a>,
which is an acronym for <strong>A</strong> <strong>L</strong>ight <strong>BERT</strong>.</li>
<li><a href="https://ai.googleblog.com/2020/08/language-agnostic-bert-sentence.html">LaBSE</a>.</li>
</ul>



See <a href="https://ai.googleblog.com/2018/11/open-sourcing-bert-state-of-art-pre.html">Open Sourcing BERT: State-of-the-Art Pre-training for Natural Language
Processing</a>
for an overview of BERT.

