#clustering

A popular [[clustering|clustering]] algorithm that groups examples
in unsupervised learning. The k-means algorithm basically does the following:

<ul>
<li>Iteratively determines the best k center points (known
as [[centroid|centroids]]).</li>
<li>Assigns each example to the closest centroid. Those examples nearest
the same centroid belong to the same group.</li>
</ul>

The k-means algorithm picks centroid locations to minimize the cumulative
<em>square</em> of the distances from each example to its closest centroid.

For example, consider the following plot of dog height to dog width:


![[ images/DogDimensions.svg ]]


If k=3, the k-means algorithm will determine three centroids. Each example
is assigned to its closest centroid, yielding three groups:


![[ images/DogDimensionsKMeans.svg ]]


Imagine that a manufacturer wants to determine the ideal sizes for small,
medium, and large sweaters for dogs. The three centroids identify the mean
height and mean width of each dog in that cluster. So, the manufacturer
should probably base sweater sizes on those three centroids. Note that
the centroid of a cluster is typically <em>not</em> an example in the cluster.

The preceding illustrations shows k-means for examples with only
two features (height and width). Note that k-means can group examples
across many features.

