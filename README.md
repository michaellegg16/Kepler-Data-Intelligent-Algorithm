# **Kepler-Data-Intelligent-Algorithm**

### Task

* The NASA Kepler Telescope has been gathering raw data for over 9 years that will be processed by creating machine learning model capable of classifying candidate exoplanets from the raw dataset. 
* In order to create the model the dataset must be preprocessed prior to fitting the model. Additionally, relevant features must be selected while also removing any unnecessary ones. 
* The MinMaxScaler function from the SciKit-learn module will be used to scale the data.
* Test_train_split is used to seperate the data into training and testing data.
* GridSearch is used to tune model parameters and select those with the best score for correctly predicting exoplanets.

### Instructions

1. Install sklearn and joblib if not already installed.
1. Read the CSV and perform basic data cleaning.
1. Select the features "'koi_fpflag_nt', 'koi_fpflag_ss', 'koi_fpflag_co'".
1. Create test_train_split using "koi_disposition" as the y-values.
1. Scale the data using the MinMaxScaler and perform feature selections.
1. Train the model and print the training and testing data scores.
1. Use GridSearchCV to tune the model's parameters.
1. Print the best scoring parameter and save the model.

### Conclusion

After tuning the model's parameters with GridSearch it was determined that a 'C' value of 1 with a gamma of 0.0001 resulted in the highest score of approximately 0.74. This is notably high considering the unreliability of data from space and the possibility of inaccurate results. Nevertheless, this model is more accurate than expected and it consistently classifies new data accurately as an exoplanet at a score just below 0.74. Comparing it to modified versions of the model using different classifiers would provide more insight. Attempting a model using multiple input parameters may also create a more accurate model. 

#### Screenshots of Results

![Data_Head](https://github.com/michaellegg16/machine-learning-challenge/blob/master/Screenshots/Data_Sample.PNG)

![Test_train](https://github.com/michaellegg16/machine-learning-challenge/blob/master/Screenshots/Test_Train_Split.PNG)

![Test_Train_Scores](https://github.com/michaellegg16/machine-learning-challenge/blob/master/Screenshots/Testing_Traing_Scores.PNG)

![Best_Params_Score](https://github.com/michaellegg16/machine-learning-challenge/blob/master/Screenshots/Best_Parameters_and_Score.PNG)
