# Apriori_Algorithm_Data_Mining
Apriori algorithm is used in mining frequent item sets and relevant association rules, describing how items are related to one another.
It works well on large datasets. For example, a real-world application may be analyzing frequent items bought in a big supermarket.

The association rules we have are:

- Support: the probability on a transaction contains items X and Y
- Confidence: the probability a transaction having X also contains Y
- Leverage: the difference between the observed frequency of X and Y appearing
together and the frequency that would be expected if X and Y were independent
- Lift and Conviction: measure of the performance of an association rule

To test this algorithm, we consider:

- The downward closure property: any subset of a frequent itemset must be frequent
- The apriori pruning principle: if there is any itemset which is infrequent, its
superset should not be generated/tested.

The candidate generation method works as follow:

- Initially, scan DB once to get frequent 1-itemset
- Generate length (k+1) candidate item sets from length k frequent item sets
- Test the candidates against DB
- Terminate when no frequent or candidate set can be generated

About dataset:

The dataset belongs to "The Bread Basket" a bakery located in Edinburgh. The dataset has 20507 entries, over 9000 transactions, and 4 columns.
It has transactions of customers who ordered different items from this bakery online and the time period of the data is from 26-01-11 to 27-12-03.
