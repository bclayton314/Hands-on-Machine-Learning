# Notes for Chapter 2

  This chapter covers an end-to-end Machine Learning project using real-world California real estate data. Considering this chapter is very hands-on, my notes might be sparse. But I will write down anything of significance.

### Steps for a Machine Learning Project:
  1. Look at the big picture.
  2. Get the data.
  3. Discover and visualize the data to gain insights.
  4. Prepare the data for Machine Learning algorithms.
  5. Select a model and train it.
  6. Fine-tune your model.
  7. Present your solution.
  8. Launch, monitor, and maintain your system.

### Frame the Problem
    -What exactly do you need to deliver?  
    -What type of problem is it?  
      -supervised, unsupervised, or Reinforcement Learning?  
      -classification, regression, something else?  
      -batch or online learning?  

**Proper definitions for RMSE and MAE, pros and cons  
### Select a Performance Measure
    -Root Mean Square Error (RMSE) - gives an idea of how much error the system typically makes in its predictions, with a higher weight for large errors.  
    -Mean Absolute Error (MAE) - less sensitive to outliers  
    Both are ways to measure the distance between two vectors: the vector of predictions and the vector of target values.  
  
### Get and Study the Data
Some useful commands for studying data in Jupyter Notebooks: .head(), info(), ds["categorical_data"].value_counts(), .describe().  
Useful visualization: .hist() (histogram)

### Create the Test Set
The book emphasizes creating the test set and making sure to not look at it otherwise it can influence the choice of ML model. This is called data snooping.  
Test sets can be 20% of the dataset but special steps must be taken to ensure the 20% test set remains isolated from the rest of the the data.
  *The book displays some useful Python functions to achieve this: the test set will remain isolated from the rest of the data using the row numbers as a unique identifier.
  *It might not be possible to use the row number as a unique identifier



## Example text
### Example text






