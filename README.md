# DATA3402-kaggle-challenge

# **Santander Customer Satisfaction challenge**

*  This repository holds an attempt to use the Santander Customer Satisfaction datasets (from kaggle), using its features of the training dataset with the "TARGET" column to predict the value of the "TARGET" column of the test dataset.

  
## Overview

* The dataset consists of mainly categorical features and is a binary classification problem. Therefore, we will use supervised machine learning algorithms (logistic regression) for this specific problem. As we have a labeled output in the training data, we will train our model with this data and try to predict an output for the "TARGET" column of the test dataset. Our best model showed an accuracy of 0.96 on training and test datasets but classified the data in the test data into one class. Using a ROC curve gave us an area of 0.56 under the graph, meaning that our model can be improved further.

## **Summary of Workdone**

## Data:
  * Type:
    * Input: CSV file of features, output: "TARGET" column
  * Size: 119.04 MB
  * Instances (Train, Test, Validation Split): The training file is split in the 2:8 ratio to make a dataset for training the model and a validation. There is a separate file for test data.

#### Preprocessing / Clean up

* Checked for null values (there weren't any).
* Dropped the ID column since it did not help in determining our output and couldn't be used as a good feature.

#### Data Visualization

* Histograms of features
* ROC curves
* Correlation matrix (Not the best looking graph)

![image](https://github.com/TajwarFahmid/DATA3402-kaggle-challenge/assets/123596299/62d62974-3468-4b09-a541-69fdf9c936ba)


### Problem Formulation

* Define:
  * The dataset consists of mainly categorical features and is a binary classification problem. Therefore, we will use supervised machine learning algorithms (logistic regression) for this specific problem. As we 
    have a labeled output in the training data, we will train our model with this data and try to predict an output for the "TARGET" column of the test dataset. Since there are a lot of features, it will be impossible to use them all so we wrote a code to identify the most important features and used the top 5.
    
  * Models
    * Linear Regression model
 

### Performance Comparison

* Used the accuracy comparison between a training and validation set, used the F1, Recall and Precision scores but they weren't of much use. Generated a ROC curve which showed an area of 0.56.

![image](https://github.com/TajwarFahmid/DATA3402-kaggle-challenge/assets/123596299/8d318bd6-1cca-4f98-8de7-1c1f41bb2133)


### Conclusions

* The model is working, but there is significant room for improvement.

### Future Work

* Computer vision, image classification.


### Data

* This data can be downloaded from kaggle, the link is at the top.



## Citations

* @misc{santander-customer-satisfaction,
    author = {Soraya_Jimenez, Will Cukierski},
    title = {Santander Customer Satisfaction},
    publisher = {Kaggle},
    year = {2016},
    url = {https://kaggle.com/competitions/santander-customer-satisfaction}
}





