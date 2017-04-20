# Coursera - Getting and Cleaning Data Course Project
The purpose of this project is to collect, work with, and clean a data set.

## Overview
This document describes the contents of this repository and the instructions to run the scripts.

## Content
1. README.md        - Describes the contents of this repository and the instructions to run the scripts.
2. run_analysis.R   - R code that perform the analysis to tidy the data and product a cleaned and aggregated data.
3. CODEBOOK.md      - Describes the variables of the tidied data set.
4. tidydata.txt     - Output of tidy data.

## Instructions
1. Download the dataset from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
2. Unzip the file and place the folder "UCI HAR Dataset" into [your R working directory].
3. Download the run_analysis.R file into [your R working directory]
4. To run the analysis, source the run_analysis.R into your R environment and then call the function runAnalysis()
5. The result table from the analysis will be written into tidydata.txt [your R working directory].

## run_analysis.R
The run_analysis.R script performs the following steps:
1. Load the activity label and feature into datasets respectively.
2. Load and merge the training, activity and subject into dataset, by filtering the features with mean and standard deviation only.
3. Load and merge the testing, activity and subject into dataset, by filtering the features with mean and standard deviation only.
4. Merge the training and testing, assign to descriptive column names.
5. Use descriptive activity names to name the activities in the merged set.
6. Create 'tidydata.txt' with the average of each variable for each activity and each subject.
