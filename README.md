# Data Science Getting and Cleaning Data Course 3 Week 4 Assignment

The purpose of this project is to collect, work and clean a data set.

Data set:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

This data is collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site :
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

Data description
----------------
The experiments have been carried out with 30 volunteers with an age group of 19-48 years. Each individual performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. This data has been provided as training/test data.

Repo has following files:
-------------------------
readme.md
CodeBook.md - description of variables
tidydata.txt - a tidy data set
run_analysis.R - R script 


Instructions for coding:
1. Merges the training and the test sets to create one data set.
   Use rbind command to merge training and test data set
2. Extracts only the measurements on the mean and standard deviation for each measurement.
   Use grep command to extract only variables that have mean() and std() in variable names.
3. Uses descriptive activity names to name the activities in the data set
   Convert acitivity label data set to one of the column name
4. Appropriately labels the data set with descriptive variable names.
   Create a new dataset that has only mean() and std() as label variables name
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
   Group the above dataset by activity names and subject name. Use summarize_all to provide mean for all variables. Result data set is tidy. data
