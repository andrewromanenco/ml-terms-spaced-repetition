#generativeAI

The process of reducing the size of one [[model|model]] (known as the
<strong>teacher</strong>) into a smaller model (known as the <strong>student</strong>) that emulates
the original model&#39;s predictions as faithfully as possible. Distillation
is useful because the smaller model has two key benefits over the larger
model (the teacher):

<ul>
<li>Faster inference time</li>
<li>Reduced memory and energy usage</li>
</ul>

However, the student&#39;s predictions are typically not as good as
the teacher&#39;s predictions.

Distillation trains the student model to minimize a
[[loss function|loss function]] based on the difference between the outputs
of the predictions of the student and teacher models.

Compare and contrast distillation with the following terms:

<ul>
<li>[[fine tuning|fine-tuning]]</li>
<li>[[prompt-based learning|prompt-based learning]]</li>
</ul>

