#fundamentals

[[feature|Features]] represented as integers or real-valued numbers.
For example, a house valuation model would probably represent the size
of a house (in square feet or square meters) as numerical data. Representing
a feature as numerical data indicates that the feature&#39;s values have
a <em>mathematical</em> relationship to the label.
That is, the number of square meters in a house probably has some
mathematical relationship to the value of the house.

Not all integer data should be represented as numerical data. For example,
postal codes in some parts of the world are integers; however, integer postal
codes shouldn&#39;t be represented as numerical data in models. That&#39;s because a
postal code of <code translate="no" dir="ltr">20000</code> is not twice (or half) as potent as a postal code of
10000. Furthermore, although different postal codes <em>do</em> correlate to different
real estate values, we can&#39;t assume that real estate values at postal code
20000 are twice as valuable as real estate values at postal code 10000.
Postal codes should be represented as [[categorical data|categorical data]]
instead.

Numerical features are sometimes called
[[continuous feature|continuous features]].

