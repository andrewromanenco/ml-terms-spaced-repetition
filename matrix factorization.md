#recsystems

In math, a mechanism for finding the matrixes whose dot product approximates a
target matrix.

In [[recommendation system|recommendation systems]], the target matrix
often holds users&#39; ratings on [[items|items]]. For example, the target
matrix for a movie recommendation system might look something like the
following, where the positive integers are user ratings and 0
means that the user didn&#39;t rate the movie:

<table>
  <tr>
    <th>&nbsp;</th>
    <th>Casablanca</th>
    <th>The Philadelphia Story</th>
    <th>Black Panther</th>
    <th>Wonder Woman</th>
    <th>Pulp Fiction</th>
  </tr>

  <tr>
    <td>User 1</td>
    <td>5.0</td>
    <td>3.0</td>
    <td>0.0</td>
    <td>2.0</td>
    <td>0.0</td>
  </tr>
  <tr>
    <td>User 2</td>
    <td>4.0</td>
    <td>0.0</td>
    <td>0.0</td>
    <td>1.0</td>
    <td>5.0</td>
  </tr>
  <tr>
    <td>User 3</td>
    <td>3.0</td>
    <td>1.0</td>
    <td>4.0</td>
    <td>5.0</td>
    <td>0.0</td>
  </tr>
</table>

The movie recommendation system aims to predict user ratings for
unrated movies. For example, will User 1 like <em>Black Panther</em>?

One approach for recommendation systems is to use matrix
factorization to generate the following two matrixes:

<ul>
<li>A [[user matrix|user matrix]], shaped as the number of users X the
number of embedding dimensions.</li>
<li>An [[item matrix|item matrix]], shaped as the number of embedding
dimensions X the number of items.</li>
</ul>

For example, using matrix factorization on our three users and five items
could yield the following user matrix and item matrix:

<pre class="prettyprint" translate="no" dir="ltr">
User Matrix                 Item Matrix

1.1   2.3           0.9   0.2   1.4    2.0   1.2
0.6   2.0           1.7   1.2   1.2   -0.1   2.1
2.5   0.5
</pre>

The dot product of the user matrix and item matrix yields a recommendation
matrix that contains not only the original user ratings but also predictions
for the movies that each user hasn&#39;t seen.
For example, consider User 1&#39;s rating of <em>Casablanca</em>, which was 5.0. The dot
product corresponding to that cell in the recommendation matrix should
hopefully be around 5.0, and it is:

<pre translate="no" dir="ltr">
(1.1 * 0.9) + (2.3 * 1.7) = 4.9
</pre>

More importantly, will User 1 like <em>Black Panther</em>? Taking the dot product
corresponding to the first row and the third column yields a predicted
rating of 4.3:

<pre translate="no" dir="ltr">
(1.1 * 1.4) + (2.3 * 1.2) = 4.3
</pre>

Matrix factorization typically yields a user matrix and item matrix that,
together, are significantly more compact than the target matrix.

