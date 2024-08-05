#language, #image

A system that learns to extract the most important information from the
input. Autoencoders are a combination of an [[encoder|encoder]] and
[[decoder|decoder]]. Autoencoders rely on the following two-step process:

<ol>
<li>The encoder maps the input to a (typically) lossy lower-dimensional
(intermediate) format.</li>
<li>The decoder builds a lossy version of the original input by mapping
the lower-dimensional format to the original higher-dimensional
input format.</li>
</ol>

Autoencoders are trained end-to-end by having the decoder attempt to
reconstruct the original input from the encoder&#39;s intermediate format
as closely as possible. Because the intermediate format is smaller
(lower-dimensional) than the original format, the autoencoder is forced
to learn what information in the input is essential, and the output won&#39;t
be perfectly identical to the input.

For example:

<ul>
<li>If the input data is a graphic, the non-exact copy would be similar to
the original graphic, but somewhat modified. Perhaps the
non-exact copy removes noise from the original graphic or fills in
some missing pixels.</li>
<li>If the input data is text, an autoencoder would generate new text that
mimics (but is not identical to) the original text.</li>
</ul>

See also [[variational autoencoder (VAE)|variational autoencoders]].

