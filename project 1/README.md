# Machine Learning Project 1 
# ** Comparison of the Results by Multiple Algorithms **
- Environment：anaconda3、jupyter notebook、python3.0
- Project library：
	
  ```
   from sklearn import svm
   from sklearn.exceptions import ChangedBehaviorWarning
   from sklearn.svm import SVC
   from sklearn.model_selection import train_test_split
   from sklearn.metrics import accuracy_score,mean_absolute_error, mean_squared_error, r2_score 
   from sklearn.linear_model import LogisticRegression,RidgeClassifier,LinearRegression
   from sklearn.neighbors import KNeighborsClassifier
   from sklearn.preprocessing import StandardScaler
   from sklearn.tree import DecisionTreeRegressor
   from sklearn.ensemble import RandomForestRegressor,GradientBoostingRegressor,GradientBoostingClassifier
   from sklearn.neural_network import MLPRegressor 

  ```
### Aim
Chosing two type projects from teacher Peter's Project Option and using different algorithms to solve them.


#### project "Housing"
1.After creating a new folder named housing, we created another new folder in this folder with the file name "data". Then we put the "housing.csv" file which we found in teacher Peter's Project Option in "data".

2.We created a new Notebook by jupyter, then we writed first code "import the pandas package and rename it as "pd". 

3.After reading "the housing.csv" file, we dicided to give each feature a column name of "RM", "LSTAT", "PTRATIO", "MEDV".

4.We used "the read_csv" to read the "housing.csv" file, and chosen first 3 columns as characteristics, while the fourth column was taken out as the column to be predicted.

5.We segmented 25% of the data for the test set and the remaining 75% for the training sample.

6.We standardized the X (it would be convenient for method 6, however， it can be done without standardization by using other methods).

7.Then we used LinearRegression, KNeighborsRegressor, DecisionTreeRegressor, RandomForestRegressor, GradientBoostingRegressor, MLPRegressor, the LogisticRegression, GradientBoostingClassifier methods to predict and calculated the mean absolute error, mean square error, and R2 coefficient of determination for each model. The GradientBoostingRegressor method was found to have the largest R2 coefficient of determination.

8.We used the GradientBoostingRegressor method was to predict RM, LSTAT, PTRATIO, MEDV respectively, and the R2 coefficient of determination was found to be different.

#### project "Classification"
1.Import the Sklear.modern_Selection function and the required libraries for classifying the data sets with four classification algorithm models.

2.Obtain pre-prepared iris data.

3.Data were divided, with training data accounting for 40%.

4.Conduct model training for four algorithms respectively.

5.Draw the line graph of the accuracy of the four models on the training set data and the test set data.

6.Take the calyx length and width as horizontal and vertical coordinates, and draw the feature classification map of the four algorithms.
<img src = "Classification\Images\1.jpg" height = "300" witdth = "500"> 
<img src = "Classification\Images\2.jpg" height = "300" witdth = "500"> 
<img src = "Classification\Images\3.jpg" height = "300" witdth = "500"> 
<img src = "Classification\Images\4.jpg" height = "300" witdth = "500"> 
<img src = "Classification\Images\5.jpg" height = "300" witdth = "500"> 


### Trouble and Solution
1. I hecked the "housing.csv" file and then list each feature. But when I print date, I fonud a problem with the contents of the data table.
<img src = "Housing\Images\trouble1.jpg" height = "300" witdth = "500"> 
Solution:Delete the first line of data from the original "housing.csv" file.

2. I used the same method to make predictions for more or less the same data, but the values of the mean absolute error, mean square error, and R2 coefficient of determination obtained were too different.。
<img src = "Housing\Images\trouble2.jpg" height = "300" witdth = "500"> 
I found that the "MEDV" column  from teacher Peter's Project Option has changed and basically expanded by a factor of nearly 10,000, so there is no problem in this case.

3. For the same set of data, I used the same method to predict different columns and found that the computed R2 coefficient of determination values were not the same.
<img src = "Housing\Images\trouble3.jpg" height = "500" witdth = "500"> 
I don't know why.


###  Summary
1. When selecting the data proportion of test set is not appropriate, the accuracy of the algorithm is very low, which makes it difficult to draw a picture.

2.Learned how to prevent Chinese characters from getting confused.Moreover, a preliminary conclusion is reached that SVM classifier and KNN classifier have the highest accuracy, followed by Logistic classifier, and Ridge classifier has the lowest accuracy when iris test data account for 40% of the total.

3.Different model algorithms for the same set of data may get different results. Therefore, it is advisable that multiple model algorithms should be used to select the optimal result. 

4.The same method to predict different feature columns for the same set of data can get different results. 
