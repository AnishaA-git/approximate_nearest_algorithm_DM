# Approximate Nearest Neighbor
An approximate nearest neighbor search algorithm is allowed to return points, whose distance from the query is at most {\displaystyle c}c times the distance from the query to its nearest points. The appeal of this approach is that, in many cases, an approximate nearest neighbor is almost as good as the exact one. In particular, if the distance measure accurately captures the notion of user quality, then small differences in the distance should not matter.

In some applications it may be acceptable to retrieve a "good guess" of the nearest neighbor. In those cases, we can use an algorithm which doesn't guarantee to return the actual nearest neighbor in every case, in return for improved speed or memory savings. Often such an algorithm will find the nearest neighbor in a majority of cases, but this depends strongly on the dataset being queried.

# Locality sensitive hashing (LSH)
Locality sensitive hashing (LSH) is a technique for grouping points in space into 'buckets' based on some distance metric operating on the points. Points that are close to each other under the chosen metric are mapped to the same bucket with high probability.

# Exhaustive Search
It is a Brute Force algorithm creates and evaluates every possible solution.

# Product Quantization
Product Quantization is a technique to reduce dataset size (from linear) by defining a function (quantizer) that encodes our data into a compact approximated representation.

# Trees and Graphs
Tree-based algorithms are one of the most common strategies when it comes to ANN. They construct forests (collection of trees) as their data structure by splitting the dataset into subsets.

# Hierarchical Navigable Small World Graphs (HNSW)
HNSW helps to tune the parameters to change the accuracy/speed tradeoff. Supports batch queries. The NSW algorithm has polylogarithmic time complexity and can outperform rival algorithms on many real-world datasets.

# Dataset
Fetch a dataset from the StackExchange network.
The datasets contain users answering questions: an interaction is defined as a user answering a given question.

The following datasets from the StackExchange network are available:
1. CrossValidated: From stats.stackexchange.com. Approximately 9000 users, 72000 questions, and 70000 answers.
2. StackOverflow: From stackoverflow.stackexchange.com. Approximately 1.3M users, 11M questions, and 18M answers.

I tried using both but the StackOverflow dataset is huge and thus takes a lot of time for further computation and processing.

## Reference
1. https://making.lyst.com/lightfm/docs/datasets.html
