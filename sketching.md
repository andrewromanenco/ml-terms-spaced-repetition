#clustering

In [[unsupervised machine learning|unsupervised machine learning]],
a category of algorithms that perform a preliminary similarity analysis
on examples. Sketching algorithms use a
<a href="https://wikipedia.org/wiki/Locality-sensitive_hashing" target="T">
locality-sensitive hash function</a>
to identify points that are likely to be similar, and then group
them into buckets.

Sketching decreases the computation required for similarity calculations
on large datasets. Instead of calculating similarity for every single
pair of examples in the dataset, we calculate similarity only for each
pair of points within each bucket.

