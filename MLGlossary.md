# **Introduction to Machine Learning** #
The machine learning (ML) approach aims at designing/programming machines/computers that can learn like a human; that is, learn from experience and discover information from the available data, but are capable of working with much larger data sets and learning at a significantly accelerated rate. The computers are programmed to optimize a performance criterion by using example data or past experience. The optimized criterion can be the accuracy provided by a predictive model — in a modelling problem — or the value of a fitness or evaluation function — in an optimization problem.<br/>
This approach is applicable to bioinformatics because the subjects are highly complex biological systems. Additionally, molecular biology that depends on a lot on experimental data can be adapted for machine learning approaches. In fact, one of the earliest application areas in machine learning was molecular biology: Stormo and his colleagues used the perceptron algorithm to locate the initial translation sites in E. coli. (Stormo et. al. 1982).

# **Why is machine learning important to bioinformatics?** #
ML techniques are highly relevant and extremely powerful in bioinformatics because they are task-oriented. Humans can understand the theoretical background and the rules generated from these techniques. Many problems in biological systems cannot be easily defined except by using examples (experimental data). Humans can specify the inputs and the corresponding output for each input, but the relationship between the inputs and outputs are often complex or unknown (e.g. the protein folding mechanism). Hence, ML approaches can be useful in such cases because they can automatically adjust their internal structure to generate approximate results for given problems. 
Another advantage of ML approaches is that they can easily be adapted to a new environment. This is important in molecular biology because new data are being generated continuously, and the newly generated data will likely update the initial concept or learning hypotheses. It is crucial for an approach or technique to be constantly revisable in order to acquire new knowledge and generate new hypotheses. This task can be accomplished easily with ML approaches due to their autonomous nature as the features can self-adapt.
Numerous ML techniques can handle many problems in bioinformatics. Logic programming, rule explanation, finite-state machines, functions system and problem solving systems being the most common ones. These techniques, operating individually or in combination, can tackle various challenges in bioinformatics.<br/>

Finally, ML can also be used for data mining. Important knowledge, relationships and correlation may remain hidden to human examination in the data. Using ML approaches to extract the (possibly) hidden information is time and cost effective, compared to manual extraction by humans.

# **Machine learning taxonomy** #
Machine learning algorithms may have different end goals that determine how the method works. 
Four main categories are: 

## [**Classification**]() ##
The computer learns from data input, and then uses the learning to categorize new observations into different groups. This may be simple (bi-class) like whether a person is male or female; or multiclass e.g. document classification. Some examples include: Linear classifiers (logistic regression, naïve Bayes classifier), Support Vector Machines, Decision Tress, Boosted Trees, Random Forest, Neural Networks, Nearest Neighbour. In the case of probabilistic classifiers such as logistic regression, the probability of predicting a class is estimated.

## [**Regression**]() ##
Regression is used to describe (or model) the relationship between the set of features (samples) in a dataset and a corresponding set of continuous numerical response variables (outputs). Some examples include simple and multiple linear regression (these fit a linear model to the input training data), ridge regression, Lasso, nearest neighbours and Kernel regression. 
| Classification | Regression |
|---|---|
| Discrete, categorical variable                      | Continuous (real number range) |
| Supervised classification problem                   | Supervised classification problem |
| Assign the output to a class (a label)              | Predict the output value using training data |
| Predict the type of tumour (harmful vs not harmful) | Predict a house price, predict survival time |


## **[Clustering]()** ## 
Clustering is an unsupervised approach that involves grouping data points according to their properties or features. Examples include K-Means clustering, Mean-Shift clustering, DBSCAN (Density-based spatial clustering of applications with noise), Expectation-Maximisation (EM) clustering using Gaussian Mixture Models (GMM), 
Agglomerative hierarchical clustering.

## **[Dimensionality reduction]()** ##
The curse of dimensionality has been one of the major problems in machine learning, which greatly alters the accuracy of a predictor. Dimension reduction has become an important technique for reducing these huge dimensions to improve predictive performance.
Feature selection can be used to filter uninformative features from the dataset, and will keep a subset of the original features. Some supervised algorithms have inbuilt feature selection, e.g. random forests and regularised regression (Ridge regression and Lasso regression). Other feature selection approaches include variance thresholds, correlation thresholds, genetic algorithms, stepwise search.

Feature extraction will make a new set of features from combinations of the original features. It can be unsupervised (e.g. Principal component analysis, PCA) or supervised (e.g. Linear discriminant analysis, LDA). 


| Supervised | Unsupervised |
|---|---|
| Input data is labelled | Input data is unlabelled |
| Uses training dataset | Uses just input dataset |
| Known number of classes | Unknown number of classes |
| Guided by expert (labelled data provided) | Self guided learning (using some criteria) |
| Goal: predict class or value label | Goal: analyse data, determine data structure/grouping |
| Classification and regression | Clustering, dimensionality reduction, density estimation |

## Choosing the right estimator 
![ML map](https://scikit-learn.org/stable/_static/ml_map.png)
Figure 1: Flowchart to choose the right estimator. Taken from: http://scikit-learn.org/stable/tutorial/machine_learning_map/index.html (website provides links to associated documentation, © 2007 - 2017, scikit-learn developers, BSD License)

# Types of Machine Learning Algorithms:
There are several main types of machine learning algorithms in common use: supervised, unsupervised, semi-supervised, reinforcement learning and statistical methods:

## i) Supervised learning approaches
These approaches use a training dataset where the outcome is known, and the relationship between a set of predictors (independent variables, risk factors) and the outcome can be modelled, and then tested on a test set as well as used to predict the outcome where it is not known.

| field1 | field2 |
|---|---|

## ii) Unsupervised learning algorithms.
These algorithms are used where there is no target or outcome variable to predict, and the primary aim is to identify clusters of items in a dataset according to specific features or characteristics. The computer learns to identify patterns in the data without human guidance about how the different clusters should be determined. 

| field1 | field2 |
|---|---|

## iii) Semi-supervised learning algorithms 
These fall between supervised and unsupervised ML algorithms, where only a subset of the data are labelled – so that where data are unlabelled, their features may still contribute understanding about the group parameters. 

| field1 | field2 |
|---|---|

## iv) Reinforcement learning algorithms
These are used to train a machine to make specific decisions and then continually improve this process through trial-and-error – learning from past experience and capturing knowledge to improve decision-making. The reinforcement learning algorithm (or agent) learns iteratively from experience, with feedback that acts as the reinforcement signal to modify the algorithm’s behaviour.

| field1 | field2 |
|---|---|

## v) Statistical methods. 

| field1 | field2 |
|---|---|

%figure (upload Fig 1b and 2)

## Summary of some applications of ML in Bioinformatics

| Type of ML | Algorithm name | Bioinformatics application [refs] |
|---|---|---|
|Supervised|Linear regression|Correlating the codon usage pattern with the protein regulation level using linear regression models [Bioinformatics study of the relationship between protein regulation and sequence properties](https://doi.org/10.1016/j.ygeno.2012.07.003)|
||Logistic Regression|Logistic regression for disease classification using microarray data: model selection in a large p and small n case [article](https://doi.org/10.1093/bioinformatics/btm287)|
||Decision Tree|Classification between disease group and non-disease group as well as to distinguish among different disease sub-types, using features generated from protein sequence and structure data [article](https://www.ncbi.nlm.nih.gov/pubmed/20139917)|
||Support Vector Machines (SVM)|Can also be used to classify between disease group and non-disease group like a Decision Tree. Other applications of SVM are: (1) prediction of membrane protein types in whole sequences. (2) prediction of translation initiation sites in biological sub-sequences [article](https://doi.org/10.1093/bib/5.4.328)|
||Naïve Bayes|Rapid Assignment of rRNA Sequences into the New Bacterial Taxonomy [article](http://aem.asm.org/content/73/16/5261.full.pdf)|
||K-Nearest Neighbour|Gene function prediction from heterogeneous data [article](https://doi.org/10.1186/1471-2105-7-S1-S11)|
||Random Forest|Used in pathway analysis and genetics association and epistasis detection [article](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3387489/)|
||Dimensionality Reduction Algorithms|E.g. PCA.  See Statistical; can be used for the visualization of microarray gene expression data [article](https://doi.org/10.1186/1471-2105-11-567).
Can also  be for biomarker discovery from high-throughput biological data [article](https://doi.org/10.1093/bib/bbn005)|
||Gradient Boosting algorithms|Predicting protein solvent accessibility which is a pivotal intermediate step towards modeling protein tertiary structures directly from one-dimensional sequences  [article](https://doi.org/10.1186/s12859-015-0851-2 )|
||Neural networks|Can be used for promoter recognition [article](https://www.ncbi.nlm.nih.gov/pubmed/2818859). Drug resistance prediction in HIV [article](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5558779/) |
||Association rules|Used to identify promising secondary phenotype candidates. Predictions rely on a large gene–phenotype annotation set that is used to find occurrence patterns of phenotypes.  [article](https://www.ncbi.nlm.nih.gov/pubmed/24932005 )|
|Unsupervised|K-means clustering|Used in gene expression studies to identify the functions of previously unstudied genes  - to reduce the data set [article](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3180043/)|
|Statistical|Principal Component Analysis|Used in studies to explain variation of gene expressions [article](https://www.ncbi.nlm.nih.gov/pubmed/21242203)|
||Independent Component Analysis||

## Glossary
|Term|Explanation|
|---|---|
|Big Data|Big data refers to large and complex datasets characterized by: (1) Volume: defines the huge amount of data that is produced. The data is so large and complex that it can no longer be saved or analyzed using conventional data processing methods. (2) Variety refers to the diversity of data types and data sources. (3) Velocity refers to the speed with which the data is generated, analyzed and reprocessed. (4) Veracity: uncertainty of data|
