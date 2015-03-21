# Introduction
 Script called run_analysis.R performs the required steps for the course project's accomplisment
 
Using the rbind() function we merge the data. We address files with the same number of columns and referring to the same entities.

We take the columns with the mean and standard deviation measures are taken from the whole dataset. Once we have taken them, we give the correct names using features.txt

As activity data is addressed with values 1:6, we take the activity names and IDs from activity_labels.txt and they are substituted in the dataset.

On the whole dataset, those columns with vague column names are corrected.

Finally, we generate a new dataset with all the average measures for each subject and activity type (30 subjects * 6 activities = 180 rows). The output file is called averages_data.txt, and uploaded to this repository.

#Variables

* x_train, y_train, x_test, y_test, subject_train and subject_train contain the data.
* x_data, y_data and subject_data merge the previous datasets to further analysis.
* features contains the correct names for the x_data dataset, which are applied to the column names stored in mean_and_std_features, a numeric vector used to extract the desired data.
* We do similarly with activity names through the activities variable.
* all_data put together x_data, y_data and subject_data 
* averages_data contains the relevant averages which will be stored in the .txt file 
*
