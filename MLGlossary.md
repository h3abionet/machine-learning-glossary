# **Introduction to Machine Learning** #
The machine learning (ML) approach aims at designing/programming machines/computers that can learn like a human; that is, learn from experience and discover information from the available data, but are capable of working with much larger data sets and learning at a significantly accelerated rate. The computers are programmed to optimize a performance criterion by using example data or past experience. The optimized criterion can be the accuracy provided by a predictive model — in a modelling problem — or the value of a fitness or evaluation function — in an optimization problem.<br/>
This approach is applicable to bioinformatics because the subjects are highly complex biological systems. Additionally, molecular biology that depends on a lot on experimental data can be adapted for machine learning approaches. In fact, one of the earliest application areas in machine learning was molecular biology: Stormo and his colleagues used the perceptron algorithm to locate the initial translation sites in E. coli. (Stormo et. al. 1982).

# **Why is machine learning important to bioinformatics?** #
ML techniques are highly relevant and extremely powerful in bioinformatics because they are task-oriented. Humans can understand the theoretical background and the rules generated from these techniques. Many problems in biological systems cannot be easily defined except by using examples (experimental data). Humans can specify the inputs and the corresponding output for each input, but the relationship between the inputs and outputs are often complex or unknown (e.g. the protein folding mechanism). Hence, ML approaches can be useful in such cases because they can automatically adjust their internal structure to generate approximate results for given problems. 
Another advantage of ML approaches is that they can easily be adapted to a new environment. This is important in molecular biology because new data are being generated continuously, and the newly generated data will likely update the initial concept or learning hypotheses. It is crucial for an approach or technique to be constantly revisable in order to acquire new knowledge and generate new hypotheses. This task can be accomplished easily with ML approaches due to their autonomous nature as the features can self-adapt.
Numerous ML techniques can handle many problems in bioinformatics. Logic programming, rule explanation, finite-state machines, functions system and problem solving systems being the most common ones. These techniques, operating individually or in combination, can tackle various challenges in bioinformatics.<br/>

Finally, ML can also be used for data mining. Important knowledge, relationships and correlation may remain hidden to human examination in the data. Using ML approaches to extract the (possibly) hidden information is time and cost effective, compared to manual extraction by humans.

# **Machine learning categories** #
Machine learning algorithms may have different end goals that determine how the method works. 
Four main categories are: 

## [**Classification**]() ##
The computer learns from data input, and then uses the learning to classify new observations into different groups. This may be simple (bi-class) like whether a person is male or female; or multiclass e.g. document classification. Some examples include: Linear classifiers (logistic regression, naïve Bayes classifier), Support Vector Machines, Decision Tress, Boosted Trees, Random Forest, Neural Networks, Nearest Neighbour. 

## [**Regression**]() ##
Regression is used to describe, or model, the relationship between the set of features in a dataset, and a continuous numerical response (output). Some examples include simple and multiple linear regression – fitting a line to the data, ridge regression, Lasso, nearest neighbours and Kernel regression. 

## **[Clustering]()** ## 
Clustering is an unsupervised approach that involves grouping data points according to their properties or features. Examples include K-Means clustering, Mean-Shift clustering, DBSCAN (Density-based spatial clustering of applications with noise), Expectation-Maximisation (EM) clustering using Gaussian Mixture Models (GMM), 
Agglomerative hierarchical clustering.

## **[Dimensionality reduction]()** ##
Feature selection can be used to filter uninformative features from the dataset, and will keep a subset of the original features. Some supervised algorithms have inbuilt feature selection, e.g. random forests and regularised regression (Ridge regression and Lasso regression). Other feature selection approaches include variance thresholds, correlation thresholds, genetic algorithms, stepwise search.




