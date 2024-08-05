#language

A technique to add information about the <em>position</em> of a token in a sequence to
the token&#39;s embedding. [[Transformer|Transformer models]] use positional
encoding to better understand the relationship between different parts of the
sequence.

A common implementation of positional encoding uses a sinusoidal function.
(Specifically, the frequency and amplitude of the sinusoidal function are
determined by the position of the token in the sequence.) This technique
enables a Transformer model to learn to attend to different parts of the
sequence based on their position.

