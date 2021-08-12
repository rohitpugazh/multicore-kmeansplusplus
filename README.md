# multicore-kmeansplusplus
This algorithm allows k-means ++ clustering for a larger number of data points efficiently.

The K-means algorithm which is one of the widely used data processing algorithms has many real-world
applications, mainly recommendation systems. However, one drawback of this algorithm is
that it takes a considerable amount of time to initialize the clusters and is not scalable for
huge datasets. The initialization in the algorithm is crucial for obtaining a good solution.
K-Means++ provides this, by locating an initial set of Centre’s that is near to the optimal
solution. However, k means++ is also a sequential algorithm and is inefficient over a large
data-set, kpasses need to be made over the entire data to find a set of good initial centres. It
is important to reduce the number of passes made to get good initialization. We have
implemented the parallel variant of the application using the MPI library along with
Clumpy and have analyzed the overall performance as well as in the hotspot regions of the
application. We intend to discuss the algorithmic complexity of both, the K-means
Clustering as well as the K-means++ algorithm highlighting the key differences between
them and justifying why the K-means++ is more scalable than its counterpart. Along with
this, we will also analyze the CPU utilization of all the 3 algorithms to be discussed in the
project and justify the results through critical evaluation. We will then perform a
comparative study with results as well as explanation of the results to justify the use of the
parallel k-means++ algorithm.
