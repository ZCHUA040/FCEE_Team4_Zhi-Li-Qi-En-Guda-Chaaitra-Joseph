# Telecom Churn Contingency

## About
This is the mini project of Group 4 from Lab Group FCEE for SC1015 (Introduction to Data Science and Artificial Intelligence).

Telecom churn refers to the phenomenon where customers switch from one telecom service provider to another. It is a problem not only in Singapore but in many different countries, this is a significant issue for telecom companies as it impacts their revenue and market share. The problem statement typically involves understanding why customers churn, predicting which customers are likely to churn in the future, and implementing strategies to reduce churn rates.

To address the problem of churn in the telecom industry, companies may employ data analytics and machine learning techniques to analyze customer data, identify churn patterns, and develop predictive models. These models can help companies proactively intervene with at-risk customers, offer targeted promotions or incentives, and improve overall customer satisfaction to reduce churn rates and increase customer retention.

## Problem Definition
- What are the main factors influencing telecom churn?
- Can we accurately predict which customers are likely to churn in the future?
- What strategies can telecom companies implement to reduce churn rates and increase customer retention?

## Dataset Used
The dataset used for this project is retrieved from [Kaggle](https://www.kaggle.com/datasets/vhcg77/telcom-churns-dataset).

## Presentation
The presentation video can be found [here](https://youtu.be/MqlNC2YfwMQ).

## Brief Process Walkthrough 

1. **Data Preparation & Cleaning**
    - Salvaged empty rows by imputing mean values
    - Removed rows with missing data after cleaning steps (Dirty data)
    - Dropped irrelevant columns
    - One-hot encoding of categorical variables
    - Generated data by upsampling minority classes to ensure overall balance.

2. **Exploratory Data Analysis**
   - Based on Demographic Predictors:
       - Equal churn rates based on gender
       - Higher churn rates observed amongst younger age groups, compared to Senior Citizens
       - Customers with partner show higher churn
       - Customers without dependants show higher churn

   - Based on Add-On Services:
       - Customers with no add-on services show higher churn
      - Customers with FibreOptics internet service show higher churn, due to high price compared to DSLOptics

   - Based on Account Information:
       - Higher customer churn observed among those with Month-to-Month contract, with median price as $80
      - Tenure predictor shows median customer churn at 10 months

   - Correlation plot: 
       - Month-To-Month Contract shows highest positive correlation (0.6)
      - Tenure shows highest negative correlation (-0.4)

  
3. **Model Training Attempt 1 with Logistic Regression** 
   - Attempted Logistic Regression
  - Train the model using feature selected from Recursive feature elimination (based on coefficient between datapoints and churn) 

     - Achieved an average accuracy score of 0.8067  and 0.8012 for train and test respectively,
     - Achieve an AUC score of  0.8352
     - Evaluated model performance:
       - Confusion Matrix
       - Recall, Precision, F1 Score
       - Receiver Operating Characteristic (ROC) Curve & Area Under Curve (AUC)
       - Model weights
      
4. **Model Training Attempt 2 with KNN Clustering**
   - Explored KNN Clustering
     - Achieved an AUC score of 0.8306
     - Evaluated model performance:
       - Confusion Matrix
       - Recall, Precision, F1 Score
       - Receiver Operating Characteristic (ROC) Curve & Area Under Curve (AUC)
       - Model weights
      
5. **Model Training Attempt 3 with Decision Tree**
   - Implemented Decision Tree
     - Trained with top 20 best predictors using K-best features.
     - Achieved an average accuracy of 0.7913 and 0.7856 for train and test set respectively.
     - Evaluated model performance:
       - Plotting decision tree
       - Confusion matrix
       - Recall, Precision, F1 Score
        
6. **Model Training Attempt 4 with Random Forest**
   - Employed Random Forest
     - Trained with top 20 best predictors using K-best features.
     - Achieved an average accuracy of 0.8044 and 0.7946 for train and test set respectively
     - Evaluated model performance:
       	- Confusion matrix
       	- Recall, Precision, F1 Score
       	- Hyper-parameter tuning using Grid search with Scoring of Accuracy and F1 Score.
    - Average accuracy of 0.8020 and 0.7970 for train and test set respectively after tuning of hyper parameters with accuracy as the scoring.
    - Average accuracy of 0.8178 and 0.8022 for train and test set respectively after tuning hyper parameters with F1 score as the scoring.

## Remodeling with Upsampled Data
1. **Re-Model Training Using Logistic Regression with Upsampled Data**
- Achieved an average accuracy score of 0.8067  and 0.8012 for train and test  respectively,
    	- Achieve an AUC score of  0.8352
      
2. **Re-Model Training using KNN Clustering with Upsampled Data**
	- Achieved an AUC score of 0.8306
      
3. **Re-Model Training using Decision Tree with Upsampled Data**
- Employed Decision Tree
	- Achieved an average accuracy of 0.7913 and 0.7856 for train and test set  respectively.
   
        
4. **Re-Model Training using Random Forest with Upsampled Data**
   - Employed Random Forest
	- Achieved an average accuracy of 0.7708 and 0.7560 for train and test set respectively
     - Evaluated model performance:
       	- Confusion matrix
       	- Hyper-parameter tuning using Grid search with Scoring of Accuracy and F1 Score.
    - Average accuracy of 0.7960 and 0.7667 for train and test set respectively after tuning of hyper parameters with accuracy as the scoring.
    - Average accuracy of 0.7976 and 0.7864 for train and test set respectively after tuning hyper parameters with F1 score as the scoring.
    
    
## Conclusion

Through our evaluation of the 4 different models of machine learning, we have concluded that using Logistic Regression will be the best option as most of the scores are similar to one another.

However, logistic regression provides coefficients for each of the features which can help in understanding the impact of each feature on the prediction better, making it more interpretable compared to random forest as it directly quantifies the impact of each feature on the predicted probability of churn.

## Key Learning Points
- Explored different modeling methods including KNN, Logistic Regression, and Random Forest
- Gained insights into Logistic regression model training & evaluation
- Explored optimization techniques for tuning hyperparameters for Random Forest
- Utilized resampling techniques to ensure a balanced view of the dataset.

## Contributors

1. [@zchua040](https://github.com/zchua040) (Chua Zhi Li) - Data Preparation & Cleaning, EDA, Model Training Attempt 1 and 2, Presentation Slides, Presenter
2. [@chaaitra001](https://github.com/chaaitra001) (Guda Chaaitra Joseph) - Model Training Attempt 3, Presentation Slides, Presenter
3. [@qchong005](https://github.com/qchong005) (Chong Qi En) - Model Training Attempt 4, Presentation Slides, Presenter
