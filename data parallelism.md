
A way of scaling [[training|training]] or [[inference|inference]]
that replicates an entire [[model|model]] onto
multiple devices and then passes a subset of the input data to each device.
Data parallelism can enable training and inference on very large
[[batch size|batch sizes]]; however, data parallelism requires that the
model be small enough to fit on all devices.

Data parallelism typically speeds training and inference.

See also [[model parallelism|model parallelism]].

<a class="glossary-anchor" name="dataset"></a>
