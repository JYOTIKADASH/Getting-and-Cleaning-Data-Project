---
title: "Code Book"
author: "J Dash"
date: "Monday, February 29, 2016"
output: html_document
---
**Per the Getting and Cleaning Data project instructions: **

The data source was downloaded and put into a folder on the local drive to have a UCI HAR Dataset folder.

the code run_analysis.R was run to generate a new file tiny_data.txt in the working directory.

The code run_analysis.R does the following:

**The training and the test sets were merged to create one data set.**

After setting the source directory for the files,the data located in features.txt,  activity_labels.txt, subject_train.txt, x_train.txt, y_train.txt, subject_test.txt, x_test.txt and y_test.txt was read into tables and assigned column names and merged to create one data set.

**Only the measurements of the mean and standard deviation for each measurement were extracted.**

This was done using the grepl function.

**Descriptive activity names were used to name the activities in the data set.**

Datasets was merged with the activity id and type table to include the descriptive activity names

**The data set was appropriately labeled with descriptive activity names.**

This was done using the melt function

**A second, independent tidy data set with the average of each variable for each activity and each subject was created.**


