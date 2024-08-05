#TensorFlow, #GoogleCloud

In ML parallel programming, a term associated with assigning the data and
model to TPU chips, and defining how these values will be sharded or replicated.

Mesh is an overloaded term that can mean either of the following:

<ul>
<li>A physical layout of TPU chips.
</li>
<li>An abstract logical construct for mapping the data and model to the TPU
chips.
</li>
</ul>

In either case, a mesh is specified as a [[shape (Tensor)|shape]].

