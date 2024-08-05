
A [[JAX|JAX]] function that splits code to run across multiple
[[accelerator chip|accelerator chips]]. The user passes a function to pjit,
which returns a function that has the equivalent semantics but is compiled
into an [[XLA (Accelerated Linear Algebra)|XLA]] computation that runs across multiple devices
(such as GPUs or [[TPU|TPU]] cores).

pjit enables users to shard computations without rewriting them by using
the [[SPMD|SPMD]] partitioner.

As of March 2023, <code translate="no" dir="ltr">pjit</code> has been merged with <code translate="no" dir="ltr">jit</code>. Refer to
<a href="https://jax.readthedocs.io/en/latest/notebooks/Distributed_arrays_and_automatic_parallelization.html">Distributed arrays and automatic
parallelization</a>
for more details.

