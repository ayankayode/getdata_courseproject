---
title: "Codebook"
author: "Kayode Ayankoya"
date: "Sunday, December 14, 2014"
output: html_document
---

## Description of Dataset

The result resulting dataset from this exercise and analysis include the combination of the training and test datasets collected from users of  SAMSUNG Galaxy S II using the embedded accelerometer and gyroscope to collect data on activities of users (WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) with the phone.


# Variable

The both of the training and the test datasets contain the following variables  
 [1] "tBodyAcc-mean()-X"          
 [2] "tBodyAcc-mean()-Y"          
 [3] "tBodyAcc-mean()-Z"          
 [4] "tBodyAcc-std()-X"           
 [5] "tBodyAcc-std()-Y"           
 [6] "tBodyAcc-std()-Z"           
 [7] "tGravityAcc-mean()-X"       
 [8] "tGravityAcc-mean()-Y"       
 [9] "tGravityAcc-mean()-Z"       
[10] "tGravityAcc-std()-X"        
[11] "tGravityAcc-std()-Y"        
[12] "tGravityAcc-std()-Z"        
[13] "tBodyAccJerk-mean()-X"      
[14] "tBodyAccJerk-mean()-Y"      
[15] "tBodyAccJerk-mean()-Z"      
[16] "tBodyAccJerk-std()-X"       
[17] "tBodyAccJerk-std()-Y"       
[18] "tBodyAccJerk-std()-Z"       
[19] "tBodyGyro-mean()-X"         
[20] "tBodyGyro-mean()-Y"         
[21] "tBodyGyro-mean()-Z"         
[22] "tBodyGyro-std()-X"          
[23] "tBodyGyro-std()-Y"          
[24] "tBodyGyro-std()-Z"          
[25] "tBodyGyroJerk-mean()-X"     
[26] "tBodyGyroJerk-mean()-Y"     
[27] "tBodyGyroJerk-mean()-Z"     
[28] "tBodyGyroJerk-std()-X"      
[29] "tBodyGyroJerk-std()-Y"      
[30] "tBodyGyroJerk-std()-Z"      
[31] "tBodyAccMag-mean()"         
[32] "tBodyAccMag-std()"          
[33] "tGravityAccMag-mean()"      
[34] "tGravityAccMag-std()"       
[35] "tBodyAccJerkMag-mean()"     
[36] "tBodyAccJerkMag-std()"      
[37] "tBodyGyroMag-mean()"        
[38] "tBodyGyroMag-std()"         
[39] "tBodyGyroJerkMag-mean()"    
[40] "tBodyGyroJerkMag-std()"     
[41] "fBodyAcc-mean()-X"          
[42] "fBodyAcc-mean()-Y"          
[43] "fBodyAcc-mean()-Z"          
[44] "fBodyAcc-std()-X"           
[45] "fBodyAcc-std()-Y"           
[46] "fBodyAcc-std()-Z"           
[47] "fBodyAccJerk-mean()-X"      
[48] "fBodyAccJerk-mean()-Y"      
[49] "fBodyAccJerk-mean()-Z"      
[50] "fBodyAccJerk-std()-X"       
[51] "fBodyAccJerk-std()-Y"       
[52] "fBodyAccJerk-std()-Z"       
[53] "fBodyGyro-mean()-X"         
[54] "fBodyGyro-mean()-Y"         
[55] "fBodyGyro-mean()-Z"         
[56] "fBodyGyro-std()-X"          
[57] "fBodyGyro-std()-Y"          
[58] "fBodyGyro-std()-Z"          
[59] "fBodyAccMag-mean()"         
[60] "fBodyAccMag-std()"          
[61] "fBodyBodyAccJerkMag-mean()" 
[62] "fBodyBodyAccJerkMag-std()"  
[63] "fBodyBodyGyroMag-mean()"    
[64] "fBodyBodyGyroMag-std()"     
[65] "fBodyBodyGyroJerkMag-mean()"
[66] "fBodyBodyGyroJerkMag-std()" 

More details about each these variables is contained in features_info.txt file available in this repo.

Moreover the following data was extracted and included in the raw data file for more description and undertanding of the data


- label   - An label of activities                    
- subject - A unique id of each participants in the experient

The label variable was extracted from the y_test/y_train files and then transformed into understandable factor by changing the values to description of each label from activity_labels.txt, thereafter, the corresponding label column was appended to the raw datasets. 

This same process was carried out for the subject to identify the recordset for each participant. The subject data was obtained from the subject file and appended to each of the datase.

**After these transformation, the test and training datasets were now joined together to form the rawdata named and outputed as rawdata.csv which was used for further analysis.**



