
Data that captures the state of a model&#39;s [[parameter|parameters]] at a
particular training iteration. Checkpoints enable exporting model
[[weight|weights]], or performing [[training|training]] across
multiple sessions. Checkpoints
also enable training to continue past errors (for example, job preemption).

When [[fine tuning|fine tuning]], the starting point for
[[training|training]] the new [[model|model]] will be a specific
checkpoint of the [[pre-trained model|pre-trained model]].

