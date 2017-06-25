#Getting-and-Cleaning-Data_Week-4-Assignment

##The repo was created for assignment for week 4 of Getting and Cleaning Data Coursera course.

Step#1: Download and unzip the data file into your R working directory.
Step#2: Download the R source code into your R working directory.
Step#3: Execute R source code file to generate tidy data file.

##Data Description

The variables in the data X are sensor signals measured with waist-mounted smartphone from 30 subjects. The variable in the data Y indicates activity type the subjects performed during recording.

##Code Description:

The code combined training dataset and test dataset, and extracted partial variables to create another dataset with the averages of each variable for each activity.

##Tidy Dataset Description:

The new generated dataset contained variables calculated based on the mean and standard deviation. Each row of the dataset is an average of each activity type for all subjects.

##Steps followed in the code to generate dataset and the output file:

1.Read training and test dataset into R environment. 
2.Merges the training and the test sets to create one data set. Use command rbind to combine training and test set
3.Extracts only the measurements on the mean and standard deviation for each measurement. Use grep command to get column indexes for variable name contains "mean()" or "std()"
4.Uses descriptive activity names to name the activities in the dataset.Convert activity labels to characters and add a new column as factor
5.Appropriately labels the data set with descriptive variable names and provide the selected descriptive names to variable columns
6.From the data set in step 4, creates a second independent tidy data set with the average of each variable for each activity and each subject.
7.Write the tidy dataset into a .txt file named tidydata.txt