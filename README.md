# Getting and Cleaning Data - Course Project

## Overview
This project demonstrates the ability to collect, work with, and clean a data set. 
The goal is to prepare tidy data that can be used for later analysis.

## Dataset
The data represents accelerometer data collected from the Samsung Galaxy S smartphone.
- Original data: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

## Files
- `run_analysis.R` - Main script that performs the analysis
- `tidy_data.txt` - The final tidy data set
- `CodeBook.md` - Describes the variables, data, and transformations

## How run_analysis.R works
The script performs the following steps:

1. **Merges** the training and test sets to create one data set
2. **Extracts** only the measurements on the mean and standard deviation for each measurement
3. **Uses descriptive activity names** to name the activities in the data set
4. **Labels** the data set with descriptive variable names
5. **Creates a second tidy data set** with the average of each variable for each activity and each subject

## How to Run
1. Download the Samsung data from the link above
2. Set your working directory to the folder containing the data
3. Run `source("run_analysis.R")`
4. The output `tidy_data.txt` will be created in your working directory

## Dependencies
- R package: `dplyr`
