# Abusive-Swearing-detection-and-clustering-demographics
### Implemented a logistic regression model and a K-Means clustering model from scratch and applied them on two real-world datasets.

#### 1. Abusive Swearing Detection  
Details:  
The dataset is a set of annotated tweets based on whether the tweet contains abusive swearing or not.  
input files:                     swad train.csv & swad test.csv.  
custom files for pre-processing: punctuations.txt & stopwords.txt.  
  
Part 1.
1. Lowercasing: Convert all the tweets into lowercase
2. Tokenization: Add space before and after punctuation present in punctuations.txt
3. Stopword removal: Remove all the stopwords present in stopwords.txt
Part 2.
1. create tfidf feature vectors from the text.
Part 3.
1. Implementing the logistic regression model, loss function as well as a parameter optimzation algorithm, e.g. stochastic gradient descent.
Part 4.
1. Evaluate the model on the test data using accuracy score as evaluation metric.


2. Clustering demographics
Details:
This partial dataset [1] contains census information including, age, workclass, education, marital status etc. The original task is to classify the people into salary brackets. We are provided with a single file (income.csv). The task is to group the data into optimum number of groups.

Part 1.\n
The dataset provided is not very clean. We do the following pre-processing steps:
1. Missing features: Replace every such feature with other values, e.g., minimum, maximum, or average of that feature.
2. Normalization: Make the range between values similar. Larger differences can make model convergence difficult.
3. Categorical features: Replace them with numerical values. e.g. male/female can be replaced with 0/1 and so on.
Part 2.
1. Implement the K-Means clustering algorithm to cluster the data into K clusters.
Part 3.
1. You should optimize the value of K using elbow method.
Part 4.
1.Create visualizations of the distortions computed by the elbow method.

References
[1] Ron Kohavi. Scaling up the accuracy of naive-bayes classifiers: A decision- tree hybrid. In Proceedings of the Second International Conference on Knowledge Discovery and Data Mining, KDD’96, page 202–207. AAAI Press, 1996.
[2] Endang Wahyu Pamungkas, Valerio Basile, and Viviana Patti. Do you re- ally want to hurt me? predicting abusive swearing in social media. In Pro- ceedings of the 12th Language Resources and Evaluation Conference, pages 6237–6246, Marseille, France, May 2020. European Language Resources As- sociation. URL https://aclanthology.org/2020.lrec-1.765.
