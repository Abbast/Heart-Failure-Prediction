# Heart Failure Prediction

## Background ## 
This is my second project within the Thinkful Data Science Flex Program curriculum. The focus of this project is the utilization of supervised learning methods (regression and/or classification) to build a model to predict some outcome for a chosen dataset.

## The Data ##
The data originates from: https://www.kaggle.com/andrewmvd/heart-failure-clinical-data. The data was collected at the Faisalabad Institute of Cardiology and Allied Hospital from April to December 2015.  

## Methods ##
As the target variable is discrete (binary), we built the following classification models prior to model selection and hyperparameter tuning
- K Nearest Neighbors (KNN)
- Random Forest
- Support Vector Machine 
- Gradient Booster

We split the data into training and test sets, with the test set comprising 20 percent of the dataset prior to training and fitting. While fitting, we used the default parameter arguments for each model to obtain a baseline for comparison.

## Evaluation ##
To assess the performance of each model, we made use of the following: accuracy, precision, and recall scores, as well as confusion matrices. The performance metrics were used to determine which baseline models could be discarded, while the confusion matrices were used to evaluate which model minimized the number of false negative (FN) classifications, i.e. stating a patient does not have heart failure when they do.

## Future Goals ##
- Rescale the variables for the models and reassess our evaluation metrics: accuracy, precision, and recall
- Build, train, and evaluate the performance of other supervised-learning models
