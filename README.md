# Telecom Churn Contingency

## About
This is the mini project of Group 4 from Lab Group FCEE for SC1015 (Introduction to Data Science and Artificial Intelligence).

Given the escalating spread of fake news amid the COVID-19 pandemic, our team decided to delve into analyzing fake news.

## Problem Definition
- TEST1
- TEST2
- TEST3 

## Dataset Used
The dataset used for this project is retrieved from [Kaggle](https://www.kaggle.com/datasets/vhcg77/telcom-churns-dataset).

## Presentation
The presentation video can be found [here](INSERT YOUR YOUTUBE LINK HERE).

## Brief Process Walkthrough 

1. **Data Preparation & Cleaning**
    - Salvaged empty rows by imputing mean values
    - Removed rows with missing data after cleaning steps (Dirty data)
    - Dropped irrelevant columns
        
    - Generated data by upsampling minority classes to ensure overall balance.

2. **Exploratory Data Analysis**
   - Conducted class analysis
   - Performed word count & character count analysis
   - Analyzed authors' contributions
   - Explored corpus statistics
   - Utilized N-gram analysis
   - Conducted sentiment & emotion analysis
   - Performed parts-of-speech (POS) analysis
   - Investigated correlation among features
  
3. **Model Training Attempt 1 with Logistic Regression** 
   - Attempted Logistic Regression
     - Achieved an average accuracy of 0.00
     - Evaluated model performance:
       - Confusion Matrix
       - Recall, Precision, F1 Score
       - Receiver Operating Characteristic (ROC) Curve & Area Under Curve (AUC)
       - Model weights
      
4. **Model Training Attempt 2 with KNN Clustering**
   - Explored KNN Clustering
     - Achieved an average accuracy of 0.00
     - Evaluated model performance:
       - Confusion Matrix
       - Recall, Precision, F1 Score
       - Receiver Operating Characteristic (ROC) Curve & Area Under Curve (AUC)
       - Model weights
      
5. **Model Training Attempt 3 with Decision Tree**
   - Implemented Decision Tree
     - Trained with top 5 predictors
     - Achieved an average accuracy of 0.00
     - Evaluated model performance:
       - Plotting decision tree
       - Confusion matrix
        
6. **Model Training Attempt 4 with Random Forest**
   - Employed Random Forest
     - Trained with top 5 predictors
     - Achieved an average accuracy of 0.00
     - Evaluated model performance:
       - Confusion matrix
       - Hyper-parameter tuning using Grid search

## Remodeling with Upsampled Data
1. **Re-Model Training Using Logistic Regression with Upsampled Data**
   - Utilized TF-IDF analysis 
   - Attempted Logistic Regression
     - Achieved an average accuracy of 0.00
     - Evaluated model performance:
       - Confusion Matrix
       - Recall, Precision, F1 Score
       - Receiver Operating Characteristic (ROC) Curve & Area Under Curve (AUC)
       - Model weights
      
2. **Re-Model Training using KNN Clustering with Upsampled Data**
   - Explored KNN Clustering
     - Achieved an average accuracy of 0.00
     - Evaluated model performance:
       - Confusion Matrix
       - Recall, Precision, F1 Score
       - Receiver Operating Characteristic (ROC) Curve & Area Under Curve (AUC)
       - Model weights
      
3. **Re-Model Training using Decision Tree with Upsampled Data**
   - Implemented Decision Tree
     - Trained with top 5 predictors
     - Achieved an average accuracy of 0.00
     - Evaluated model performance:
       - Plotting decision tree
       - Confusion matrix
        
4. **Re-Model Training using Random Forest with Upsampled Data**
   - Employed Random Forest
     - Trained with top 5 predictors
     - Achieved an average accuracy of 0.00
     - Evaluated model performance:
       - Confusion matrix
       - Hyper-parameter tuning using Grid search

## Conclusion
- Testing

## Key Learning Points
- Explored different modeling methods including KNN, Logistic Regression, and Random Forest
- Gained insights into Logistic regression model training & evaluation
- Explored optimization techniques for tuning hyperparameters for Random Forest
- Utilized resampling techniques to ensure a balanced view of the dataset.

## Contributors

1. [@zchua040](https://github.com/zchua040) (Chua Zhi Li) - Data Preparation & Cleaning, Exploratory Data Analysis, Presentation Slides, Model Training Attempt 1 and 2
2. [@chaaitra001](https://github.com/chaaitra001) (Guda Chaaitra Joseph) - Model Training Attempt 3, Presentation Slides, Presenter
3. [@qchong005](https://github.com/qchong005) (Chong Qi En) - Model Training Attempt 4, Presentation Slides, Presenter

## References
- List any references here.
