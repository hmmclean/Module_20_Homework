## Module_20_Homework
Module 20 - Supervised Machine Learning

## Overview
This historical dataset of lending activity from a peer-to-peer lending services company was used to build a model that can identify the creditworthiness of borrowers. This dataset was imported into a pandas data frame and separated into two variables (x and y). These variables were further split into training data and testing data to allow the models to learn using the training data and then test accuracy and precision with the testing data. Logistic regression models were used with the original data to predict healthy loan and high-risk loan labels. The data was then resampled and the logistic regression model was retrained with the resampled data to address class imbalance and predict healthy loan and high-risk loan labels. 

## Navigation
* Credit_Risk 
    * lending_data - provided csv dataset.
    * credit_risk_classification - provided jupyter notebook file that contains the code.
* README - contains final analysis.
* report-template - template for analysis report.

## Analysis

* Explain the purpose of the analysis.
     * The primary objective of this analysis was to develop a predictive model for assessing the creditworthiness of borrowers using a historical dataset obtained from a peer-to-peer lending services company. 
* Explain what financial information the data was on, and what you needed to predict.
     * The dataset contains lending activity records and serves as the basis for predicting the creditworthiness of borrowers. Two main variables, loan status (y) and all other features (x), were derived from the dataset. The focus of the analysis was on predicting   healthy loans and high-risk loans so that decisions can be made around risk management associated with these classifications. 
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
     * The variables to predict, representing loan labels, were categorized as "healthy loan" and "high-risk loan." There were 75,036 healthy loans and 2,500 high-risk loans. Exploring the distribution of these labels through methods like value_counts provided insights into the dataset's class distribution and whether the distribution was appropriate.
* Describe the stages of the machine learning process you went through as part of this analysis.
     * The machine learning process involved several key stages. Firstly, the dataset was imported into a pandas data frame. Following this, the data was divided into two variables (x and y) and further split into training and testing sets. Logistic regression models were then applied to the original data for initial predictions. Subsequently, recognizing the need to address class imbalance, the data underwent resampling. The logistic regression model was retrained using the resampled data to enhance its performance in predicting both healthy and high-risk loan classifications.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
     * The logistic regression algorithm was a central component of the analysis, utilized initially with the original dataset and subsequently with the resampled data. Resampling methods were employed to tackle the imbalance of the initial model predominantly identifying loans as low-risk, ensuring a more robust prediction of loan labels.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Model 1 Balanced Accuracy Score: 0.95
  * Model 1 Confusion Matrix:
       * True Negatives: 18663
       * True Positives: 563
       * False Negatives: 56
       * False Positives: 102
  * Classification Report:
       * Model 1 Accuracy: 0.99
       * Model 1 Precision:
            * Healthy Loans (0): 1.00
            * High-risk Loans (1): 0.85
       * Model 1 Recall scores:
            * Healthy Loans (0): 0.99
            * High-risk Loans (1): 0.91


* Machine Learning Model 2:
   * Model 2 Balanced Accuracy Score: 0.99
   * Model 2 Confusion Matrix:
       * True Negatives: 18649
       * True Positives: 615
       * False Negatives: 4
       * False Positives: 116
   * Classification Report:
       * Model 2 Accuracy: 0.99
       * Model 2 Precision:
            * Healthy Loans (0): 1.00
            * High-risk Loans (1): 0.84
       * Model 2 Recall scores:
            * Healthy Loans (0): 1.00
            * High-risk Loans (1): 0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
I would recommend model 2, with the resampled data because it has the lowest false negatives, which would mean predicting high risk loans as healthy. 
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
  

# References and Resources
* ChatGPT - https://chat.openai.com/
