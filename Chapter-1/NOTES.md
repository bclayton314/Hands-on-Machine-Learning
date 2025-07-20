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
* One important parameter of online learning systems is how fast they should adapt to changing data: this is called the learning rate. If you set a high learning rate, then your system will rapidly adapt to new data, but it will also tend to quickly forget the old data (you don’t want a spam filter to flag only the latest kinds of spam it was shown). Conversely, if you set a low learning rate, the system will have more inertia; that is, it will learn more slowly, but it will also be less sensitive to noise in the new data or to sequences of nonrepresentative data points (outliers).

### Instance-Based Versus Model-Based Learning
Instance-based learning: the system learns examples by heart, then generalizes to new cases by using a similarity measure to compare them to the learned examples (or a subset of them).

Model-based learning: build a model from a set of examples and use that model to make predictions.

## Challenges in ML
-Insufficient Quantity of Training Data  
-Nonrepresentative Training Data  
-Poor-Quality Data  
-Irrelevant Features  
-Overfitting the Training Data - the model performs well on the training data, but it does not generalize well.  
-Underfitting the Training Data - occurs when your model is too simple to learn the underlying structure of the data.  

*Overfitting happens when the model is too complex relative to the amount and noisiness of the training data. Here are possible solutions:  
  • Simplify the model by selecting one with fewer parameters
  (e.g., a linear model rather than a high-degree polynomial
  model), by reducing the number of attributes in the training
  data, or by constraining the model.  
  • Gather more training data.  
  • Reduce the noise in the training data (e.g., fix data errors and
  remove outliers).  

*Here are the main options for fixing underfitting:  
  • Select a more powerful model, with more parameters.  
  • Feed better features to the learning algorithm (feature engineering).  
  • Reduce the constraints on the model (e.g., reduce the regularization hyperparameter).  

*The Unreasonable Effectiveness of Data - algorithms are important, but good quality data is more important.  

## Testing and Validating
-Training set / Test set  
-Cross-validation  
-Validation set
-Train-dev set

### Other vocabulary
attribute: a data type.  
feature: an attribute plus its value.  
labels: the correct or expected output values associated with input data, used to train supervised learning models. They provide the ground truth that the model learns to predict or classify. Essentially, labels are the answers to the questions the model is trying to learn to answer.  
Dimensionality reduction: the goal is to simplify the data without losing too much information. One way to do this is to merge several correlated features into one.  
Association Rule Learning: the goal is to dig into large amounts of data and discover interesting relations between attributes.  
Out-of-Core Learning: Online learning algorithms that can be used to train systems on huge datasets that cannot fit in one machine’s main memory. The algorithm loads part of the data, runs a training step on that data, and repeats the process until it has run on all of the data. Incremental learning.  
Feature selection: selecting the most useful features to train on among existing features.  
Feature extraction: combining existing features to produce a more useful one—as we saw earlier, dimensionality reduction algorithms can help.  
Regularization: Constraining a model to make it simpler and reduce the risk of overfitting.  
Hyperparameter: a parameter of a learning algorithm (not of the model). As such, it is not affected by the learning algorithm itself; it must be set prior to training and remains constant during training.  





