#TensorFlow

Describes the information required to extract [[feature|features]] data
from the [[tf.Example|tf.Example]] protocol buffer. Because the
tf.Example protocol buffer is just a container for data, you must specify
the following:

<ul>
<li>The data to extract (that is, the keys for the features)</li>
<li>The data type (for example, float or int)</li>
<li>The length (fixed or variable)</li>
</ul>

