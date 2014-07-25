## Getting and Cleaning Data Course Project


Contains the R-code used for data cleaning with description of variables &amp; steps taken to do so. 

## Purpose of this project 

To demonstrate my ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis.

##  Expected Results.

 R script called run_analysis.R should be created which would do the following. 

* Merges the training and the test sets to create one data set.
    
* Extracts only the measurements on the mean and standard deviation for each measurement. 
    
* Uses descriptive activity names to name the activities in the data set
    
* Appropriately labels the data set with descriptive variable names. 
    
* Creates a second, independent tidy data set with the average of each variable for each activity and each subject.



##Dependencies/R Packages required. 

* reshape2

* data.table

Note: Make sure that the UCI HAR Dataset folder is in the Working Directory.

## Steps taken to achieve the expected results.

1. Load the following files into R using read.table fuction.

* activity_labels.txt

* features.txt

* X_test.txt & Y_test.txt

* X_train.txt & Y_train.txt

2. Extract only the measurements on the mean and standard deviation using grepl function.

3.Column Bind the test & train data so that it contains all the features, subject, Avtivity ID and the Activity Label.

4. Merge the test and train data from step 4 using the rbind function

5. Use the melt function to make a tidy dataset that clearly shows the id labels vs the measured labels/columns.

6. Use the dcast function to get a second, independent tidy data set with the average of each variable for each activity and each subject.

##codebook.md

Contains detailed description of the variables, the data, and any transformations or work that was performed to clean up the data.

##run_analysis.R 

Contains the R Script employed to get the expected results.



