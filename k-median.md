#clustering

A clustering algorithm closely related to [[k-means|k-means]]. The
practical difference between the two is as follows:

<ul>
<li>In k-means, centroids are determined by minimizing the sum of the
<em>squares</em> of the distance between a centroid candidate and each of
its examples.</li>
<li>In k-median, centroids are determined by minimizing the sum of the
distance between a centroid candidate and each of its examples.</li>
</ul>

Note that the definitions of distance are also different:

<ul>
<li>k-means relies on the
<a href="https://wikipedia.org/wiki/Euclidean_distance"
target="T">Euclidean distance</a> from
the centroid to an example. (In two dimensions, the Euclidean
distance means using the Pythagorean theorem to calculate
the hypotenuse.) For example, the k-means distance between (2,2)
and (5,-2) would be:</li>
</ul>

<div>
$$
{\text{Euclidean distance}} = {\sqrt {(2-5)^2 + (2--2)^2}} = 5
$$
</div>

<ul>
<li>k-median relies on the <a href="https://wikipedia.org/wiki/Taxicab_geometry"
target="T"> Manhattan distance</a>
from the centroid to an example. This distance is the sum of the
absolute deltas in each dimension. For example, the k-median
distance between (2,2) and (5,-2) would be:</li>
</ul>

<div>
$$
{\text{Manhattan distance}} = \lvert 2-5 \rvert + \lvert 2--2 \rvert = 7
$$
</div>


