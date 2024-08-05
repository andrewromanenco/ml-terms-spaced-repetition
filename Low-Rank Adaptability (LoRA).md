#language, #generativeAI

An algorithm for performing
[[parameter-efficient tuning|parameter efficient tuning]] that
[[fine tuning|fine-tunes]] only a subset of a
[[large language model|large language model&#39;s]] parameters.
LoRA provides the following benefits:

<ul>
<li>Fine-tunes faster than techniques that require fine-tuning <em>all</em> of a model&#39;s
parameters.</li>
<li>Reduces the computational cost of [[inference|inference]] in the
fine-tuned model.</li>
</ul>

A model tuned with LoRA maintains or improves the quality of its predictions.

LoRA enables multiple specialized versions of a model.



