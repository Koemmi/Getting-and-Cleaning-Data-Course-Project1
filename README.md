# Getting and Cleaning Data - Course Project

- This repository was built for the course project of the "Getting and Cleaning Data" course at Coursera. 

- The goal of this project is to create a tidy data data set with the help of R to analyze experimental results which were captured in the [Human Activity Recognition Using Smartphones] (http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones) study.

- The data for this project can be downloaded through the following link:   https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

## Repository Information

This repository contains 4 main files:

1. `README.md`: explains how all of the scripts work and how they are connected.

2. `CodeBook.md`: a code book that describes the variables, the data, and any transformations or work that we performed to clean up the data.

3. `run_analysis.R`: this script is used to generate the tidy data set from raw data recorded in the *Human Activity Recognition Using Smartphones Data Set*. The process of generating tidy data set includes the following steps:

   - Merges the training and the test sets to create one data set called `mergedata`.
   - Extracts only the measurements on the mean and standard deviation for each measurement to get `feature_mean_std`.
   - Uses descriptive activity names to name the activities in the data set, replace `activity_id` with descriptive names in `activity_label`.
   - Appropriately labels the data set with descriptive variable names given in `feature_name`.
   - From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject `unique_act_sub`.

4. `tidy_dataset.txt`: is the exported final data after going through all the sequences described above.
