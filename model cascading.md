#generativeAI

A system that picks the ideal [[model|model]] for a specific inference
query.

Imagine a group of models, ranging from very large (lots of
[[parameter|parameters]]) to much smaller (far fewer parameters).
Very large models consume more computational resources at
[[inference|inference]] time than smaller models. However, very large
models can typically infer more complex requests than smaller models.
Model cascading determines the complexity of the inference query and then
picks the appropriate model to perform the inference.
The main motivation for model cascading is to reduce inference costs by
generally selecting smaller models, and only selecting a larger model for more
complex queries.

Imagine that a small model runs on a phone and a larger version of that model
runs on a remote server. Good model cascading reduces cost and latency by
enabling the smaller model to handle simple requests and only calling the
remote model to handle complex requests.

See also [[model router|model router]].

