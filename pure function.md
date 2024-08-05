
A function whose outputs are based only on its inputs, and that has no side
effects. Specifically, a pure function doesn&#39;t use or change any global state,
such as the contents of a file or the value of a variable outside the function.

Pure functions can be used to create thread-safe code, which is beneficial
when sharding [[model|model]] code across multiple
[[accelerator chip|accelerator chips]].

[[JAX|JAX&#39;s]] function transformation methods require
that the input functions are pure functions.


