#language, #image, #generativeAI

A second, task-specific training pass performed on a
[[pre-trained model|pre-trained model]] to refine its parameters for a
specific use case. For example, the full training sequence for some
[[large language model|large language models]] is as follows:

<ol>
<li><strong>Pre-training:</strong> Train a large language model on a vast <em>general</em> dataset,
such as all the English language Wikipedia pages.</li>
<li><strong>Fine-tuning:</strong> Train the pre-trained model to perform a <em>specific</em> task,
such as responding to medical queries. Fine-tuning typically involves
hundreds or thousands of examples focused on the specific task.</li>
</ol>

As another example, the full training sequence for a large image model is as
follows:

<ol>
<li><strong>Pre-training:</strong> Train a large image model on a vast <em>general</em> image
dataset, such as all the images in Wikimedia commons.</li>
<li><strong>Fine-tuning:</strong> Train the pre-trained model to perform a <em>specific</em> task,
such as generating images of orcas.</li>
</ol>

Fine-tuning can entail any combination of the following strategies:

<ul>
<li>Modifying <em>all</em> of the pre-trained model&#39;s existing
[[parameter|parameters]]. This is sometimes called <strong>full fine-tuning</strong>.</li>
<li>Modifying only <em>some</em> of the pre-trained model&#39;s existing parameters
(typically, the layers closest to the [[output layer|output layer]]),
while keeping other existing parameters unchanged (typically, the layers
closest to the [[input layer|input layer]]). See
[[parameter-efficient tuning|parameter-efficient tuning]].</li>
<li>Adding more layers, typically on top of the existing layers closest to the
output layer.</li>
</ul>

Fine-tuning is a form of [[transfer learning|transfer learning]].
As such, fine-tuning might use a different loss function or a different model
type than those used to train the pre-trained model. For example, you could
fine-tune a pre-trained large image model to produce a regression model that
returns the number of birds in an input image.



Compare and contrast fine-tuning with the following terms:

<ul>
<li>[[distillation|distillation]]</li>
<li>[[prompt-based learning|prompt-based learning]]</li>
</ul>

