Codebook for PA1 - Getting and Cleaning Data
========

## Data was obtained from the source below
## Human Activity Recognition Using Smartphones Dataset
## Version 1.0
Jorge L. Reyes-Ortiz, Davide Anguita, Alessandro Ghio, Luca Oneto.
Smartlab - Non Linear Complex Systems Laboratory
DITEN - Universit? degli Studi di Genova.
Via Opera Pia 11A, I-16145, Genoa, Italy.
activityrecognition@smartlab.ws
www.smartlab.ws

# Data processing
- Data was downloaded from "https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip"
- Data was unzipped
- Column Name changes from Features downloaded files for the 561 columns was performed by removing dashes and keeping names under lower cap
- Both test and train sets were processed separate in order to match individual and activity rows per set
- Train and Test set were binded by rows
- For extraction of measurement wit mean and std only grepping was used then data was subset for the index columns
- On the subsetted files Individual and Activity variable were converted to factor and Activity was transfor from numerical to a more descriptive term
- Tidy set was generated by using the aggregate function using only the first five columns, script can be modified to include more. but for ease of evaluation only five are included
- Tidy set was exported as a comma delimited file.


## Variables used and processed for the Merged train and test set were:
The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain. See 'features_info.txt' for more details. 

 [1] "tbodyaccmean()x"               
 [2] "tbodyaccmean()y"               
 [3] "tbodyaccmean()z"               
 [4] "tgravityaccmean()x"            
 [5] "tgravityaccmean()y"            
 [6] "tgravityaccmean()z"            
 [7] "tbodyaccjerkmean()x"           
 [8] "tbodyaccjerkmean()y"           
 [9] "tbodyaccjerkmean()z"           
[10] "tbodygyromean()x"              
[11] "tbodygyromean()y"              
[12] "tbodygyromean()z"              
[13] "tbodygyrojerkmean()x"          
[14] "tbodygyrojerkmean()y"          
[15] "tbodygyrojerkmean()z"          
[16] "tbodyaccmagmean()"             
[17] "tgravityaccmagmean()"          
[18] "tbodyaccjerkmagmean()"         
[19] "tbodygyromagmean()"            
[20] "tbodygyrojerkmagmean()"        
[21] "fbodyaccmean()x"               
[22] "fbodyaccmean()y"               
[23] "fbodyaccmean()z"               
[24] "fbodyaccmeanfreq()x"           
[25] "fbodyaccmeanfreq()y"           
[26] "fbodyaccmeanfreq()z"           
[27] "fbodyaccjerkmean()x"           
[28] "fbodyaccjerkmean()y"           
[29] "fbodyaccjerkmean()z"           
[30] "fbodyaccjerkmeanfreq()x"       
[31] "fbodyaccjerkmeanfreq()y"       
[32] "fbodyaccjerkmeanfreq()z"       
[33] "fbodygyromean()x"              
[34] "fbodygyromean()y"              
[35] "fbodygyromean()z"              
[36] "fbodygyromeanfreq()x"          
[37] "fbodygyromeanfreq()y"          
[38] "fbodygyromeanfreq()z"          
[39] "fbodyaccmagmean()"             
[40] "fbodyaccmagmeanfreq()"         
[41] "fbodybodyaccjerkmagmean()"     
[42] "fbodybodyaccjerkmagmeanfreq()" 
[43] "fbodybodygyromagmean()"        
[44] "fbodybodygyromagmeanfreq()"    
[45] "fbodybodygyrojerkmagmean()"    
[46] "fbodybodygyrojerkmagmeanfreq()"
[47] "tbodyaccstd()x"                
[48] "tbodyaccstd()y"                
[49] "tbodyaccstd()z"                
[50] "tgravityaccstd()x"             
[51] "tgravityaccstd()y"             
[52] "tgravityaccstd()z"             
[53] "tbodyaccjerkstd()x"            
[54] "tbodyaccjerkstd()y"            
[55] "tbodyaccjerkstd()z"            
[56] "tbodygyrostd()x"               
[57] "tbodygyrostd()y"               
[58] "tbodygyrostd()z"               
[59] "tbodygyrojerkstd()x"           
[60] "tbodygyrojerkstd()y"           
[61] "tbodygyrojerkstd()z"           
[62] "tbodyaccmagstd()"              
[63] "tgravityaccmagstd()"           
[64] "tbodyaccjerkmagstd()"          
[65] "tbodygyromagstd()"             
[66] "tbodygyrojerkmagstd()"         
[67] "fbodyaccstd()x"                
[68] "fbodyaccstd()y"                
[69] "fbodyaccstd()z"                
[70] "fbodyaccjerkstd()x"            
[71] "fbodyaccjerkstd()y"            
[72] "fbodyaccjerkstd()z"            
[73] "fbodygyrostd()x"               
[74] "fbodygyrostd()y"               
[75] "fbodygyrostd()z"               
[76] "fbodyaccmagstd()"              
[77] "fbodybodyaccjerkmagstd()"      
[78] "fbodybodygyromagstd()"         
[79] "fbodybodygyrojerkmagstd()"     
[80] "activity"                      
[81] "individual"                  

