# **Hepatitis-Mortality-Analysis**

Predicting Hepatitis Mortality from the uci dataset (https://archive.ics.uci.edu/ml/datasets/hepatitis)

## **Description**

In this paper we process and analyze data concerning Hepatitis. The data was taken from the UCI and analyzed with the help of the Python language.In order to process them corectly,we use methods such as feature selection, oversampling and categorization models such as Naïve Bayes, Support Vector Machines, Logistic Regression and Decision Trees. To evaluate their performance we use cross validation and after comparing the results, we can see which method performs best for this particular dataset .
 
## **I.  Introduction**

After we have entered the data we begin the process of analysis and processing. After pre-processing our data and bringing it to the best possible form, we start modeling the classifiers for training and testing our models. More specifically, we try to compare the methods in order to find out the best method by applying the models to two different datasets. The original set with 19 features and the "processed" one with the best 12 features. At the same time for their evaluation, given our choice of feature selection we choose the method of cross validation.

## **II.  Metholodology**

To evaluate our models, we used cross validation, which is a reliable method of evaluating the classification as it divides the data into K parts using each time k-1 for training the model and k part for its validation. Classification report was selected as an output, as it gives us information on the performance of the model in 3 different metric (macro, micro, weighted ). For the evaluation and comparison of classification models, we focus mainly on accuracy and sensitivity. While for selecting the best value for k folds, we focus on Cross Validation Accuracy Score.

### **A.  Data**

In order to precess our data we need to bring it from a csv into a Dataframe format.We continue by replacing the "?" values with "0" and define the type of our datatset's features.

### **B. Classification Techniques**

- **Gaussian Naïve Bayes** (For reducing computional complexity, increasing speed and minimizing ranking error)
- **Support Vector Machines** (For clasifiaction and regression problems)
- **Logistic Regression** (with maximum likelihood estimation for minimizing the ranking error)
- **Decission Trees** (CA.R.T.)

### **C.  Description of the most Effective Method**
Initially the UCI dataset contains samples from 155 patients suffering from hepatitis and categorizes them into two classes: "Live" and "Die",by considering its 19 features.
By analyzing the distribution of our data, we notice an unequal distribution between the two classes with patients in the "Live" category touching 79 % .
