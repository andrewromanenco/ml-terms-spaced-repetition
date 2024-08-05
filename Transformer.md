#language

A [[neural network|neural network]] architecture developed at Google that
relies on [[self-attention (also called self-attention layer)|self-attention]] mechanisms to transform a
sequence of input embeddings into a sequence of output
embeddings without relying on [[convolution|convolutions]] or
[[recurrent neural network|recurrent neural networks]]. A Transformer can be
viewed as a stack of self-attention layers.

A Transformer can include any of the following:

<ul>
<li>an [[encoder|encoder]]</li>
<li>a [[decoder|decoder]]</li>
<li>both an encoder and decoder</li>
</ul>

An <strong>encoder</strong> transforms a sequence of embeddings into a new sequence of the
same length. An encoder includes N identical layers, each of which contains two
sub-layers. These two sub-layers are applied at each position of the input
embedding sequence, transforming each element of the sequence into a new
embedding. The first encoder sub-layer aggregates information from across the
input sequence. The second encoder sub-layer transforms the aggregated
information into an output embedding.

A <strong>decoder</strong> transforms a sequence of input embeddings into a sequence of
output embeddings, possibly with a different length. A decoder also includes
N identical layers with three sub-layers, two of which are similar to the
encoder sub-layers. The third decoder sub-layer takes the output of the
encoder and applies the [[self-attention (also called self-attention layer)|self-attention]] mechanism to
gather information from it.

The blog post <a href="https://ai.googleblog.com/2017/08/transformer-novel-neural-network.html">Transformer: A Novel Neural Network Architecture for Language
Understanding</a>
provides a good introduction to Transformers.

