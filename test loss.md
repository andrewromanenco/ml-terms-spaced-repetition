#fundamentals

A [[metric|metric]] representing a model&#39;s [[loss|loss]] against
the [[test set|test set]]. When building a [[model|model]], you
typically try to minimize test loss. That&#39;s because a low test loss is a
stronger quality signal than a low [[training loss|training loss]] or
low [[validation loss|validation loss]].

A large gap between test loss and training loss or validation loss sometimes
suggests that you need to increase the
[[regularization rate|regularization rate]].

