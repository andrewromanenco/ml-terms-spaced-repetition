#language

A Python-first [[configuration|configuration]] library that sets the
values of functions and classes without invasive code or infrastructure.
In the case of [[Pax|Pax]]—and other ML codebases—these functions and
classes represent [[model|models]] and [[training|training]]
[[hyperparameter|hyperparameters]].

<a href="https://github.com/google/fiddle" target="T">Fiddle</a>
assumes that machine learning codebases are typically divided into:

<ul>
<li>Library code, which defines the layers and optimizers.</li>
<li>Dataset &quot;glue&quot; code, which calls the libraries and wires everything together.</li>
</ul>

Fiddle captures the call structure of the glue code in an unevaluated and
mutable form.

