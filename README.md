# Getting and Cleaning Data
Third course in the Data Science Specialization on Coursera

* This repository contains the Course Project related to this course through Johns Hopkins University
* The script "run_analysis.R" is cleaning data collected from accelerometers of the Samsung Galaxy S smartphone
  * It merges the training and the test sets into one data set
  * It extracts only the measurements on the mean and standard deviation for each measurement
  * It uses descriptive activity names to name the activities in the data set
  * It appropriately labels the data set with descriptive activity names
  * And it creates an independent tidy data set with the average of each variable, each activity and each subject
  
* You can find all project-related materials in the UCI HAR Dataset directory
* However, copies of the important files have been put into this main directory to fulfill the submission requirement

* Unzip (https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip)
* Put "run_analysis.R" into the "UCI HAR Dataset" folder
* In RStudio: Set your working directory to the "UCI HAR Dataset" folder
* Execute: source("run_analysis.R")
* Followed by: data <- read.table("data_set_with_the_averages.txt") 
* To view my tidy data: View(data)

* It is 180x68 because there are 30 subjects and 6 activities.
* Thus "for each activity and each subject" means 30 * 6 = 180 rows. 
* Note that the provided R script has no assumptions on numbers of records, only on locations of files.
