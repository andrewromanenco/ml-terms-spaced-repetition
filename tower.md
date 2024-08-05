
A component of a [[deep neural network|deep neural network]] that is
itself a deep neural network. In some cases, each tower reads from an
independent data source, and those towers stay independent until their
output is combined in a final layer. In other cases, (for example, in
the [[encoder|encoder]] and [[decoder|decoder]] stack/tower of
many [[Transformer|Transformers]]), towers have cross-connections
to each other.

