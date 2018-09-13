## First, what is Clustering?
**Clustering** consists of discovering the inherent groupings in a dataset, *i.e* partitioning a set of elements into subsets, called clusters, according to the differences and similarties between them without any prior knowledge about the data structure. <br/>
A good clustering result maximises homogeneity between intra group and  separability between the different groups. 

## Assess the quality of a clustering algorithm results is important to avoid finding random patterns in data. 

**Internal cluster validation:** uses only internal information to the clustering process without reference to external information, it is based on inter-clusters separability and intra-clusters homogenity. Clusters should be well-separated (inter-cluster distance should be maximized) and intra-cluster distance should be small.<br/>

**External cluster validation:** compares results to an externally known results (example: class labels), compare different clustering methods results, etc. <br/>
**Relative cluster validation:** evaluates the clustering methods by varying different parameters values for the same algorithm (example:number of clusters)<br/> 

**Example in bioinformatics**
One of the most popular applications of clusering in bioinformatics is the the clustering of genes based on their expression profiles. In RNA-seq experiments we obtain the expression value for thousands of genes in a few samples. An interesting insight that we can extract from this data is which genes are co-expressed in the different samples.  This is a clustering problem where genes with similar expression levels in all samples are grouped into a cluster.


