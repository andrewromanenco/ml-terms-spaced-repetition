#language

A form of [[model parallelism|model parallelism]] in which a model&#39;s
processing is divided into consecutive stages and each stage is executed
on a different device. While a stage is processing one batch, the preceding
stage can work on the next batch.

See also [[staged training|staged training]].

