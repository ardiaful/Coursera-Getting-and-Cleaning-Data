##Introduction

Raw data are obtained from UCI Machine Learning repository, particularly the Human Activity Recognition Using Smartphones Data Set.

The data set was built from experiments carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (walking, walking upstairs, walking downstairs, sitting, standing, laying) wearing 
a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, 3-axial linear acceleration and 3-axial angular velocity were captured at a constant rate of 50Hz. The data obtained has been randomly partitioned into two sets, where 70% of the volunteers were selected for generating the training data and 30% the test data.

##Variables

1. The following variables contain the data from the downloaded files:x_train, y_train, x_test, y_test, subject_train and subject_test.

2. x_data, y_data and subject_data merge the previous datasets to further analysis.

3. features contains the correct names for the x_data dataset, which are applied to the column names stored in mean_and_std_features, a numeric vector used to extract the desired data.

4. A similar approach is taken with activity names through the activities variable.

5. all_data merges x_data, y_data and subject_data in a big dataset.

6. Finally, averages_data contains the relevant averages which will be later stored in a .txt file. 

7. ddply() from the plyr package is used to apply colMeans() and ease the development.
