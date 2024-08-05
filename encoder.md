#language

In general, any ML system that converts from a raw, sparse, or external
representation into a more processed, denser, or more internal representation.

Encoders are often a component of a larger model, where they are frequently
paired with a [[decoder|decoder]]. Some [[Transformer|Transformers]]
pair encoders with decoders, though other Transformers use only the encoder
or only the decoder.

Some systems use the encoder&#39;s output as the input to a classification or
regression network.

In [[sequence-to-sequence task|sequence-to-sequence tasks]], an encoder
takes an input sequence and returns an internal state (a vector). Then, the
[[decoder|decoder]] uses that internal state to predict the next sequence.

Refer to [[Transformer|Transformer]] for the definition of an encoder in
the Transformer architecture.

