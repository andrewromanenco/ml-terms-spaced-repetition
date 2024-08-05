#recsystems

An algorithm for minimizing the objective function during
[[matrix factorization|matrix factorization]] in
[[recommendation system|recommendation systems]], which allows a
downweighting of the missing examples. WALS minimizes the weighted
squared error between the original matrix and the reconstruction by
alternating between fixing the row factorization and column factorization.
Each of these optimizations can be solved by least squares
[[convex optimization|convex optimization]]. For details, see the
<a href="/machine-learning/recommendation/collaborative/matrix"
   target="T"
   class="gc-analytics-event"
   data-category="launchRecommendationCourse"
   data-label="ml-glossary"
   data-action="click">Recommendation Systems course</a>.

