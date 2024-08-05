#language, #image, #generativeAI

A [[model|model]] that infers a prediction based on its own previous
predictions. For example, auto-regressive language models predict the next
[[token|token]] based on the previously predicted tokens.
All [[Transformer|Transformer]]-based
[[large language model|large language models]] are auto-regressive.

In contrast, [[GAN|GAN]]-based image models are usually not auto-regressive
since they generate an image in a single forward-pass and not iteratively in
steps. However, certain image generation models <em>are</em> auto-regressive because
they generate an image in steps.

