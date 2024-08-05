
Overloaded term that could be used in any of the following ways:

<ul>
<li>Implementing [[quantile bucketing|quantile bucketing]]
on a particular [[feature|feature]].</li>
<li>Transforming data into zeroes and ones for quicker storing, training,
and inferring. As Boolean data is more robust to noise and errors than
other formats, quantization can improve model correctness.
Quantization techniques include rounding, truncating, and
[[binning|binning]].</li>
<li>Reducing the number of bits used to store a model&#39;s
[[parameter|parameters]]. For example, suppose a model&#39;s parameters are
stored as 32-bit floating-point numbers. Quantization converts those
parameters from 32 bits down to 4, 8, or 16 bits. Quantization reduces the
following:

<ul>
<li>Compute, memory, disk, and network usage</li>
<li>Time to infer a predication</li>
<li>Power consumption</li>
</ul>

However, quantization sometimes decreases the correctness of a model&#39;s
predictions.
</li>
</ul>

