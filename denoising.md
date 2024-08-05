#language

A common approach to [[self-supervised learning|self-supervised learning]]
in which:

<ol>
<li>[[noise|Noise]] is artificially added to the dataset.</li>
<li>The [[model|model]] tries to remove the noise.</li>
</ol>

Denoising enables learning from [[unlabeled example|unlabeled examples]].
The original [[data set or dataset|dataset]] serves as the target or
[[label|label]] and
the noisy data as the input.

Some [[masked language model|masked language models]] use denoising
as follows:

<ol>
<li>Noise is artificially added to an unlabeled sentence by masking some of
 the tokens.</li>
<li>The model tries to predict the original tokens.</li>
</ol>

