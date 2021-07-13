# Heart Failure Prediction

## Background ## 
This is my second project within the Thinkful Data Science Flex Program curriculum. The focus of this project is the utilization of supervised learning methods (regression and/or classification) to build a model to predict some outcome for a chosen dataset.

## The Data ##
The data originates from: https://www.kaggle.com/andrewmvd/heart-failure-clinical-data. The data was collected at the Faisalabad Institute of Cardiology and Allied Hospital from April to December 2015.  

### Description of the Features
We include the following description of the features and their dimensions, where appropriate.

* Age: the age of the patient (years)
* Anaemia: the decrease of red blood cells or hemoglobin
  
    0 = `no`, 1 = `yes`
* Creatinine Phosphokinase: Level of the CPK enzyme in the blood (mcg/L)
* Diabetes: If the patient has diabetes
    
    0 = `no`, 1 = `yes`
* Ejection Fraction: Percentage of blood leaving the heart at each contraction (percentage)
* High Blood Pressure: If the patient has hypertension
* Platelets: Platelets in the blood (kiloplatelets/mL)
* Serum Breatinine: Level of serum creatinine in the blood (mg/dL)
* Serum Sodium: Level of serum sodium in the blood (mg/dL)
* Sex: Gender of the patient 
   
   0 = `Female`, 1 = `Male`
* Smoking: Does the patient smoke?
    
    0 = `no`, 1 = `yes`
* Time: Follow-up period

### Demographic Information
As the dataset pertains to heart failure, it contains demographic features that we can examine further to obtain a better understanding of the data. The features of interest include the following: 

- Age
- Sex
- Anaemia
- Diabetes
- High Blood Pressure
- Smoking

To gain a better grasp on features, we used plotted either histograms or pie charts, depending on whether the variable was continuous or discretized.

![](../raw/master/Images/ImportantImage.png)

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
