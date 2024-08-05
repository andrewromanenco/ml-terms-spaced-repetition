#TensorFlow, #GoogleCloud

When training an ML model on [[accelerator chip|accelerator chips]]
(GPUs or [[TPU|TPUs]]), the part of the system
that controls both of the following:

<ul>
<li>The overall flow of the code.</li>
<li>The extraction and transformation of the input pipeline.</li>
</ul>

The host typically runs on a CPU, not on an accelerator chip; the
[[device|device]] manipulates [[Tensor|tensors]] on the
accelerator chips.

