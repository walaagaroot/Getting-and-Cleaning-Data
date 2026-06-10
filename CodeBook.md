# CodeBook

## Overview
This codebook describes the variables, data, and transformations performed 
to clean up the data for the Getting and Cleaning Data Course Project.

## Source Data
- Original data: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
- Description: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

## Variables

### Identifiers
- `subject` - ID of the test subject (1-30)
- `activity` - Type of activity performed:
  - WALKING
  - WALKING_UPSTAIRS
  - WALKING_DOWNSTAIRS
  - SITTING
  - STANDING
  - LAYING

### Measurements
All measurement variables are the **average** of each variable for each activity and each subject.

- `TimeBodyAccelerometer-mean()-XYZ` - Mean body acceleration (time domain)
- `TimeBodyAccelerometer-std()-XYZ` - Std deviation body acceleration (time domain)
- `TimeGravityAccelerometer-mean()-XYZ` - Mean gravity acceleration (time domain)
- `TimeBodyAccelerometerJerk-mean()-XYZ` - Mean body jerk acceleration (time domain)
- `TimeBodyGyroscope-mean()-XYZ` - Mean body gyroscope (time domain)
- `TimeBodyGyroscopeJerk-mean()-XYZ` - Mean body gyroscope jerk (time domain)
- `TimeBodyAccelerometerMagnitude-mean()` - Mean body acceleration magnitude
- `FrequencyBodyAccelerometer-mean()-XYZ` - Mean body acceleration (frequency domain)
- `FrequencyBodyGyroscope-mean()-XYZ` - Mean body gyroscope (frequency domain)

## Transformations
1. Training and test sets were merged into one data set
2. Only mean and standard deviation measurements were extracted
3. Activity codes were replaced with descriptive activity names
4. Variable names were made descriptive:
   - `t` prefix replaced with `Time`
   - `f` prefix replaced with `Frequency`
   - `Acc` replaced with `Accelerometer`
   - `Gyro` replaced with `Gyroscope`
   - `Mag` replaced with `Magnitude`
   - `BodyBody` replaced with `Body`
5. Final data set contains the average of each variable grouped by subject and activity
6. 
