# NLP---Topic-Modeling-NMF

## NMF is little bit faster than LDA for topic modeling in maximum cases

NMF has an inherent clustering property,[15] i.e., it automatically clusters the columns of input data {\displaystyle \mathbf {V} =(v_{1},\cdots ,v_{n})}\mathbf {V} =(v_{1},\cdots ,v_{n}).

More specifically, the approximation of {\displaystyle \mathbf {V} }\mathbf {V}  by {\displaystyle \mathbf {V} \simeq \mathbf {W} \mathbf {H} }\mathbf {V} \simeq \mathbf {W} \mathbf {H}  is achieved by finding {\displaystyle W}W and {\displaystyle H}H that minimize the error function

{\displaystyle ||V-WH||_{F},}{\displaystyle ||V-WH||_{F},} subject to {\displaystyle W\geq 0,H\geq 0.}W\geq 0,H\geq 0.

If we furthermore impose an orthogonality constraint on {\displaystyle \mathbf {H} }\mathbf {H} , i.e. {\displaystyle \mathbf {H} \mathbf {H} ^{T}=I}{\displaystyle \mathbf {H} \mathbf {H} ^{T}=I}, then the above minimization is mathematically equivalent to the minimization of K-means clustering [15].

Furthermore, the computed {\displaystyle H}H gives the cluster membership, i.e., if {\displaystyle \mathbf {H} _{kj}>\mathbf {H} _{ij}}{\displaystyle \mathbf {H} _{kj}>\mathbf {H} _{ij}} for all i ≠ k, this suggests that the input data {\displaystyle v_{j}}v_{j} belongs to {\displaystyle k^{th}}k^{{th}} cluster. The computed {\displaystyle W}W gives the cluster centroids, i.e., the {\displaystyle k^{th}}k^{{th}} column gives the cluster centroid of {\displaystyle k^{th}}k^{{th}} cluster. This centroid's representation can be significantly enhanced by convex NMF.

When the orthogonality constraint {\displaystyle \mathbf {H} \mathbf {H} ^{T}=I}{\displaystyle \mathbf {H} \mathbf {H} ^{T}=I} is not explicitly imposed, the orthogonality holds to a large extent, and the clustering property holds too. Clustering is the main objective of most data mining applications of NMF

source :https://en.wikipedia.org/wiki/Non-negative_matrix_factorization
