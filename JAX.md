
An array computing library, bringing together
[[XLA (Accelerated Linear Algebra)|XLA (Accelerated Linear Algebra)]] and automatic differentiation
for high-performance numerical computing. JAX provides a simple and powerful
API for writing accelerated numerical code with composable transformations.
JAX provides features such as:

<ul>
<li><code translate="no" dir="ltr">grad</code> (automatic differentiation)</li>
<li><code translate="no" dir="ltr">jit</code> (just-in-time compilation)</li>
<li><code translate="no" dir="ltr">vmap</code> (automatic vectorization or batching)</li>
<li><code translate="no" dir="ltr">pmap</code> (parallelization)</li>
</ul>

JAX is a language for expressing and composing transformations of numerical
code, analogous—but much larger in scope—to Python&#39;s [[NumPy|NumPy]]
library. (In fact, the .numpy library under JAX is a functionally equivalent,
but entirely rewritten version of the Python NumPy library.)

JAX is particularly well-suited for speeding up many machine learning tasks
by transforming the models and data into a form suitable for parallelism
across GPU and [[TPU|TPU]] [[accelerator chip|accelerator chips]].

[[Flax|Flax]], [[Optax|Optax]], [[Pax|Pax]], and many other
libraries are built on the JAX infrastructure.


