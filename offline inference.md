#fundamentals

The process of a model generating a batch of [[prediction|predictions]]
and then caching (saving) those predictions. Apps can then access the inferred
prediction from the cache rather than rerunning the model.

For example, consider a model that generates local weather forecasts
(predictions) once every four hours. After each model run, the system
caches all the local weather forecasts. Weather apps retrieve the forecasts
from the cache.

Offline inference is also called <strong>static inference</strong>.

Contrast with [[online inference|online inference]].

