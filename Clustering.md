## First, what is Clustering
**Clustering** consists of discovering the inherent groupings in a dataset, *i.e* partitioning a set of elements into subsets according to the differences and similarties between them. In other words, it is the process of grouping similar elements together into clusters. The main difference from the supervised classification is that, in clustering, we have no information about how many classes there are. A good clustering result maximises homogeneity between intra group and  separability between the different groups. 

**Example in bioinformatics**
Clustering of genes in expression data - In RNA-seq experiments we obtain the expression value for thousands of genes in a few samples. An interesting insight that we can extract from this data is which genes are co-expressed in the different samples.  This is a clustering problem where genes with similar expression levels in all samples are grouped into a cluster.

## Assess the quality of a clustering algorithm results is important to avoid finding random patterns in data. 

**Internal cluster validation:** uses only internal information to the clustering process without reference to external information (clusters separability, clusters homogenity, etc.)
Clusters should be well-separated and intra-cluster distance should be small

**External cluster validation:** compares results to an externally known results (example: class labels), compare different clustering methods results, etc.
**Relative cluster validation:** evaluates the clustering methods by varying different parameters values for the same algorithm (example:number of clusters) 
