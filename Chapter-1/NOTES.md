# Notes for Chapter 1

## Types of ML Systems
### 4 Main Types: Supervised Learning, Unsupervised Learning, Semisupervised, and Reinforcement Learning
Supervised Learning: the training set is already labeled. Typical supervised learning tasks: classification or prediction.  
Examples: spam filter or car price prediction using regression.  
Some of the most important supervised learning algorithms: k-Nearest Neighbors, Linear Regression, Logistic Regression, Support Vector Machines (SVM), Decision Trees and Random Forests, Neural Networks

Unsupervised Learning: the training data is unlabeled. The system tries to learn without a teacher.  
Some of the most important unsupervised learning algorithms:  
• Clustering  
  —K-Means  
  —DBSCAN  
  —Hierarchical Cluster Analysis (HCA)  
• Anomaly detection and novelty detection  
  —One-class SVM  
  —Isolation Forest  
• Visualization and dimensionality reduction  
  —Principal Component Analysis (PCA)  
  —Kernel PCA  
  —Locally Linear Embedding (LLE)  
  —t-Distributed Stochastic Neighbor Embedding (t-SNE)  
• Association rule learning  
  —Apriori  
  —Eclat  

Semisupervised Learning: Some algorithms can deal with data that’s partially labeled. Most semisupervised learning algorithms are combinations of unsupervised and supervised algorithms. For example, deep belief networks (DBNs) are based on unsupervised components called restricted Boltzmann machines (RBMs) stacked on top of one another. RBMs are trained sequentially in an unsupervised manner, and then the whole system is fine-tuned using supervised learning techniques.

Reinforcement Learning: The learning system, called an agent in this context, can observe the environment, select and perform actions, and get rewards in return (or penalties in the form of negative rewards).

### Batch and Online Learning
In batch learning, the system is incapable of learning incrementally: it must be trained using all the available data. This will generally take a lot of time and computing resources, so it is typically done offline. First the system is trained, and then it is launched into production and runs without learning anymore; it just applies what it has learned. This is called offline learning.

In online learning, you train the system incrementally by feeding it data instances sequentially, either individually or in small groups called mini-batches. Each learning step is fast and cheap, so the system can learn about new data on the fly.


### Other vocabulary
attribute: a data type.  
feature: an attribute plus its value.  
labels: the correct or expected output values associated with input data, used to train supervised learning models. They provide the ground truth that the model learns to predict or classify. Essentially, labels are the answers to the questions the model is trying to learn to answer.  
Dimensionality reduction: the goal is to simplify the data without losing too much information. One way to do this is to merge several correlated features into one.  
Association Rule Learning: the goal is to dig into large amounts of data and discover interesting relations between attributes.  


## Challenges in ML


## Testing and Validating



